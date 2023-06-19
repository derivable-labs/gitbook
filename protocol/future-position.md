# Future Position

Users can add extra locktime to the maturity duration when opening a position, effectively converting it into a futures position. Futures position benefit from the `DiscountRate`, as the LP interest will not be charged for a portion of the locktime.

$$InterestFreeDuration = Locktime \times DiscountRate$$

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

For example, suppose a pool has a Discount Rate of 75%. If a user opens a LONG or SHORT position with an additional locktime of 4 days, no interest rate will be applied during the first 3 days of the locktime.
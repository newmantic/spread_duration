# spread_duration

The spread duration is a measure used in fixed income to assess how sensitive the price of a bond is to changes in its credit spread. Credit spread is the difference in yield between a bond with credit risk (such as a corporate bond) and a risk-free bond (like a government bond) of similar maturity. Spread duration is particularly useful for bonds that have credit risk and helps investors understand how changes in credit spreads impact the value of their investments.


Credit Spread (S):
The difference between the yield on a bond with credit risk and a risk-free bond. It compensates investors for taking on the additional credit risk.

Yield to Maturity (Y):
The total return anticipated on a bond if it is held until it matures. This includes interest payments (coupons) and the difference between the bond's purchase price and its face value.

Bond Price (P):
The current market price of the bond, which is the present value of its expected cash flows (coupons and face value) discounted by the yield to maturity.


Spread duration D_s  can be expressed as:
D_s = − (ΔP/P)/ΔS
Where:
ΔP is the change in bond price.
P is the initial bond price.
ΔS is the change in credit spread.

Approximation Using Finite Differences
Since the changes in P and S are typically small, spread duration can be approximated using finite differences:
D_s ≈ − ( P(S+ΔS) − P(S−ΔS) ) / 2⋅P⋅ΔS
Where:
P(S+ΔS) is the bond price when the spread increases by ΔS.
P(S−ΔS) is the bond price when the spread decreases by ΔS.

Bond Price Calculation
The price of a bond P given its yield to maturity Y and spread S can be calculated as:
P = ∑_{t=1}^{T} C/((1+Y+S)^t) + F/((1+Y+S)^T)
Where:
C is the annual coupon payment.
T is the number of years to maturity.
F is the face value of the bond.

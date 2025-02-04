# FractionalFee

A fraction of the transferred units of a token to assess as a fee. The amount assessed will never be less than the given minimum\_amount, and never greater than the given maximum\_amount. The denomination is always units of the token to which this fractional fee is attached.

| Field | Type | Description |
| :--- | :--- | :--- |
| `fractional_amount` | [Fraction](../../basic-types/fraction.md) | The fraction of the transferred units to assess as a fee |
| `minimum_amount`  | int64 | The minimum amount to assess |
| `maximum_amount` | int64 | The maximum amount to assess \(zero implies no maximum\) |
| `net_of_transfers` | bool | If true, assesses the fee to the sender, so the receiver gets the full amount from the token transfer list, and the sender is charged an additional fee; if false, the receiver does NOT get the full amount, but only what is left over after paying the fractional fee |


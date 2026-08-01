# GPO Processing Order (LSDOU)

## Order

Local

↓

Site

↓

Domain

↓

OU

## Rule

If multiple GPOs configure the same setting, the last applied policy normally takes precedence.

## Lab

Created two wallpaper policies.

Domain = Blue

HR = Green

Result:

HR wallpaper was applied because the OU policy was processed after the domain policy.

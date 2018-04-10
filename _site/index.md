# API
[Documentation](https://statsmachina.docs.apiary.io/)

# Google Sheets add-on
[Link](https://chrome.google.com/webstore/detail/stats-machina/obkacnpchmodnejaeaedjmleaphfojbi?utm_source=permalink) | [Functions Reference](#functions-reference)

## Functions Reference

```ruby
AB_CONFIDENCE(control_users, control_conversions, variant_users, variant_conversions, confidence_level)
```

> Returns the confidence level: percentage chance that the observed uplift is statistically significant.

Parameters ([definitions](#definitions)):
- [x] `control_users` -- required
- [x] `control_conversions` -- required
- [x] `variant_users` -- required
- [x] `control_conversions` -- required
- [ ] `confidence_level` -- optional

```ruby
AB_UPLIFT(control_users, control_conversions, variant_users, variant_conversions)
```

> Returns the uplift in conversion rates between control and a variant.

Parameters ([definitions](#definitions)):
- [x] `control_users` -- required
- [x] `control_conversions` -- required
- [x] `variant_users` -- required
- [x] `control_conversions` -- required

```ruby
AB_CONVERSIONRATE(users, conversions)
```

> Returns the conversion rate of a variant.

Parameters ([definitions](#definitions)):
- [x] `users` -- required
- [x] `conversions` -- required

# Definitions

- `users` -- The number of unique users who met the targeting criteria to enter the test.
- `conversions` -- The number of unique conversions (i.e. number of users who completed a goal at least once).
- `confidence_level` -- Default: 0.95 -- The level of confidence required to deem an observed uplift statistically significant.
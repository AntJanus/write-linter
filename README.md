# Write Linter

## To do

- come up with a better name

## How does the linting work?

- count % of overused words VS total (overused words take up 5% of total)
- top word frequency (not linting, but a statistic that would be available "writing coverage")
- throw error when a "no-no" word is used
- keep writing above a certain grade level
- fail CI when rules are broken

## Available rules

1. % usage of a crutch word
2. usage of "no-no" word
3. grade level (min, max)
4. basic checks (used the same word twice by accident, period AFTER quote, etc.)

## Config file

```js
{
  crutchPercent: 5,
  crutchDictionary: './resources/crutchwords.js',
  nonoWords: true,
  nonoDictionary: './resources/nonowords.js',
  minGradeLevel: 5,
  maxGradeLevel: 9,
  basicCheck: true
}
```

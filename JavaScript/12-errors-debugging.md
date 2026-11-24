# 12 — Errors and debugging

## Common errors
- `SyntaxError`: code cannot be parsed.
- `ReferenceError`: a name cannot be resolved.
- `TypeError`: an operation is invalid for a value.
- `RangeError`: a value is outside an allowed range.

## try / catch / finally

```javascript
try {
  const value = JSON.parse("{invalid}");
  console.log(value);
} catch (error) {
  console.error("Could not parse JSON:", error.message);
} finally {
  console.log("Finished");
}
```

## Throw

```javascript
function divide(a, b) {
  if (b === 0) throw new Error("Cannot divide by zero");
  return a / b;
}
```

## Debugging tools
- `console.log()`: inspect values.
- `console.table()`: display tabular data.
- `console.error()`: report errors.
- Breakpoints: pause execution.
- Step over / into / out: follow execution.
- Call stack: inspect function calls.
- Network panel: inspect requests.

## Workflow
1. Reproduce the problem.
2. Read the exact error and stack trace.
3. Identify the line and relevant values.
4. Form one hypothesis.
5. Test a small change.
6. Verify the fix and check for regressions.

## Practice
Intentionally create a TypeError, inspect the console, and fix it.

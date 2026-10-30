# Everyday Calculator

A small, browser-only calculator for addition, subtraction, multiplication, and division. It also handles decimal numbers and parentheses, works with the keyboard, and keeps calculations on your device. There is no build step, account, or saved history.

## Run it

1. Open `index.html` in a modern browser.
2. Select the calculator buttons or type a calculation on your keyboard.
3. Press **=** or **Enter** to see the answer.
4. Use **C** or **Esc** to start over. The backspace button removes the last character.

The arithmetic logic is kept in the independently usable `CalculatorMath` object in `script.js`. For example, in the browser developer console:

```js
CalculatorMath.calculate("18 + 24"); // 42
CalculatorMath.calculate("96 ÷ 8");  // 12
CalculatorMath.calculate("7 × 6");   // 42
```

## Manual checks

- On a fresh page, the display is empty and shows its starting hint.
- Enter `18 + 24`, `96 ÷ 8`, and `7 × 6`; confirm the results are `42`, `12`, and `42`.
- Enter `2 + 3 × 4`; confirm multiplication happens first and the answer is `14`.
- Try `(2 + 3) × 4`; confirm parentheses produce `20`.
- Try `8 ÷ 0`; confirm an inline division-by-zero message appears.
- Try a decimal calculation such as `.5 + 1.25`; confirm the answer is `1.75`.
- Check **C**, backspace, keyboard **Enter**, keyboard **Esc**, and the mobile layout.

## Beginner Git practice

Git helps you save named checkpoints as you learn. Open a terminal in this project folder and try:

```text
git status
git add index.html styles.css script.js README.md
git status
git commit -m "Build a simple browser calculator"
git log -1 --oneline
```

`git status` shows which files changed, `git add` stages the files for a checkpoint, and `git commit` saves that checkpoint with a message. If Git says your name or email is not configured, ask your instructor or follow your organization's Git setup instructions before committing.

AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA

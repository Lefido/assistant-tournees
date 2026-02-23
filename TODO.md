# Fix: "Sélectionnez un bras de distribution" overflow issue

## Problem
The label "Sélectionnez un bras de distribution" is overflowing the "main-content" block at the top.

## Root Cause
- `.main-content` has `height: 100vh` with `overflow: hidden`
- `#userPanel` has `margin-top: -20px` which pushes content upward
- This causes the title to be pushed outside the visible area

## Solution Plan
- [x] Analyze the CSS and identify the issue
- [ ] Change `.main-content` from `height: 100vh` to `min-height: 100vh` to allow content expansion
- [ ] Test the fix

## Files to Edit
- style.css: Modify `.main-content` height property

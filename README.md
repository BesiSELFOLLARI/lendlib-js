# lendlib-js
Small reusable JavaScript library for tracking lent books. It exposes `window.LendLib`.

## Usage
Add this before your own script:

```html
<script src="https://cdn.jsdelivr.net/gh/BesiSELFOLLARI/lendlib-js@v1.0.1/lendlib.js"></script>
```

## API
- `LendLib.validate(data)` returns the list of missing required fields
- `LendLib.create(data)` returns a new loan object
- `LendLib.isOverdue(loan)` and `LendLib.getStatus(loan)`
- `LendLib.summary(loans)` returns `{ total, overdue }`
- `LendLib.save(loans)` and `LendLib.load()` use localStorage
- `LendLib.escapeHtml(text)` makes text safe to put in HTML
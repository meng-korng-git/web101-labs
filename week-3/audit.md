# Accessibility Audit Report

## Website Audited

YouTube Homepage

---

## 1. Lighthouse Accessibility Score

* Accessibility Score: **89/100**

### Failed Audits

* Some buttons do not have accessible names
* Low color contrast in some areas
* Missing form labels
* Links are not clearly descriptive

---

## 2. axe DevTools Results

### Critical Issues

1. Images missing alternative text (`alt`)
2. Form inputs without labels

### Serious Issues

1. Poor color contrast
2. Heading levels skipped
3. Buttons missing accessible names

---

## 3. Keyboard Navigation Test

When using the **Tab** key to navigate through the homepage, the focus is mostly visible. However, some buttons and links are difficult to notice because the outline color is too light.

---

# Top 3 Accessibility Issues and Suggested Fixes

## Issue 1: Missing Alternative Text

Some images do not include descriptive `alt` text, making it difficult for screen readers.

### Suggested Fix

Add meaningful `alt` attributes to all images.

```html
<img src="logo.png" alt="YouTube Logo">
```

---

## Issue 2: Low Color Contrast

Some text colors blend into the background and are hard to read.

### Suggested Fix

Use darker text or lighter backgrounds to improve readability.

---

## Issue 3: Form Inputs Missing Labels

Search bars or form fields are missing proper labels.

### Suggested Fix

Use the `<label>` element correctly.

```html
<label for="search">Search</label>
<input type="text" id="search">
```
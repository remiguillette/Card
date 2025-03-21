
# Test Page Debug Information

## CSS File Contents (static/css/test/test_page.css)

```css
/* Custom Font Declarations */
@font-face {
    font-family: 'Tahoma';
    src: url('/static/assets/Tahoma.woff2') format('woff2');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Tahoma-Bold';
    src: url('/static/assets/Tahoma-Bold.woff2') format('woff2');
    font-weight: bold;
    font-style: normal;
    font-display: swap;
}

/* CSS Variables */
:root {
    --blue-color: #0d6efd;
    --orange-color: #f89422;
    --black-color: #000000;
}

/* Base styles */
* {
    -webkit-user-modify: read-only;
    -moz-user-modify: read-only;
    user-modify: read-only;
    -webkit-user-select: none;
    -moz-user-select: none;
    user-select: none;
}

html, body {
    margin: 0;
    padding: 0;
    overflow: hidden;
    height: 100vh;
    font-family: 'Tahoma', sans-serif;
}

/* Layout */
.content-container {
    display: flex;
    width: 100vw;
    height: 100vh;
    position: relative;
    overflow: hidden;
}

.left-panel {
    position: absolute;
    left: 0;
    top: 0;
    width: 50%;
    height: 100%;
    background-color: var(--black-color);
    padding: min(2vw, 2rem);
    color: var(--orange-color);
    font-size: min(2vw, 24px);
    overflow-y: auto;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    text-align: left;
    gap: 1vh;
}

.right-panel {
    position: absolute;
    right: 0;
    top: 0;
    width: 50%;
    height: 100%;
    background-color: var(--orange-color);
    padding: min(2vw, 2rem);
    color: var(--black-color);
    font-size: min(2vw, 24px);
    overflow-y: auto;
}

/* Text styles */
.name-title, .large-name {
    display: flex;
    align-items: center;
    justify-content: flex-start;
    gap: 10px;
    width: 100%;
    text-align: left;
}

.left-panel .name-title, .left-panel .large-name {
    flex-direction: row;
}

.name-title {
    margin: 0;
    font-size: min(6.8vw, 6.8rem);
}

.large-name {
    font-size: min(6.875vw, 6.875rem);
    margin: 0;
    font-family: 'Tahoma-Bold', sans-serif;
}

.first, .last {
    font-weight: 700;
}

.first {
    color: var(--blue-color);
}

.last {
    color: var(--orange-color);
}

.text-group {
    color: var(--orange-color);
    margin-bottom: clamp(0.5rem, 1vw, 1rem);
    font-size: clamp(32px, 4vw, 48px);
}

.company-text {
    color: var(--orange-color);
    margin-bottom: clamp(0.5rem, 1vw, 1rem);
    font-size: clamp(32px, 4vw, 48px);
}

.right-title {
    font-family: 'Tahoma-Bold', sans-serif;
    font-size: 4rem;
    margin-bottom: 1rem;
    font-weight: 700;
}

.right-subtitle {
    font-family: 'Tahoma-Bold', sans-serif;
    font-size: 4rem;
    margin-bottom: 2rem;
    font-weight: 700;
}

.right-info {
    font-size: 3rem;
    margin-bottom: 1rem;
}

/* Ontario Pride section */
.ontario-pride {
    display: flex;
    flex-direction: row;
    align-items: left;
    justify-content: flex-start;
    gap: clamp(1rem, 2vw, 2rem);
    margin-top: clamp(1rem, 2vw, 2rem);
    width: 100%;
}

.ontario-pride::before {
    content: '';
    background-image: url('/static/assets/beaver.png');
    background-size: contain;
    background-repeat: no-repeat;
    background-position: left;
    width: clamp(60px, 10vw, 120px);
    height: clamp(60px, 10vw, 120px);
    flex-shrink: 0;
    filter: invert(57%) sepia(87%) saturate(1401%) hue-rotate(346deg) brightness(101%) contrast(94%);
}

.ontario-pride::after {
    content: 'Proud to be Ontarian\A Fiers d\'être Ontariens';
    white-space: pre;
    color: var(--orange-color);
    font-size: clamp(24px, 3vw, 43px);
    line-height: 1.2;
}

/* Responsive design */
@media (max-width: 768px) {
    .left-panel {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 50%;
    }

    .right-panel {
        position: absolute;
        top: 50%;
        left: 0;
        width: 100%;
        height: 50%;
    }
}
```

## Browser Console Output
No errors are currently displayed in the browser console.

## Network Tab Status
- File: `/static/css/test/test_page.css`
- Status: 200 OK
- Type: text/css
- Size: 4.2 KB

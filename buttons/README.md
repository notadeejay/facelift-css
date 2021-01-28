## General Implementation notes

- For the most part button sizing / responsiveness / positioning should stay roughly the same, I tried not to change to much from the existing implementation.

## top-button

This is the button that appears at the right hand side of the lesson page and says **Go to current**. New HTML should be as follows. Changed the SVG and swaped the order of the SVG and label:
```html
<div class="lesson-part__topButton"><button
                        type="button" class="top-button"><span
                            class="top-button__icon"><svg width="18"
                                height="21" viewBox="0 0 18 21"
                                fill="none"
                                xmlns="http://www.w3.org/2000/svg">
                                <path d="M2 9L9 2M9 2L16 9M9 2V19.5"
                                    stroke="#039BE8" stroke-width="3"
                                    stroke-linecap="round"
                                    stroke-linejoin="round" />
                            </svg></span> <span
                            class="top-button__label">Go to
                            Current</span>
                    </button></div>
```

## launch button
- Added SVGs as the button backgrounds
- Wrapped inside of a new div `launch__wrapper`
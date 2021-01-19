## Lesson Modal


## Lab Modal

### HTML Changes

Remove the `lab-congrats__embed` div

```html
<div class="lab-congrats__embed">
                                <div class="ff-container ff-ready ff-inactive"
                                    tabindex="0">
                                    <div class="ff-overlay">
                                    </div><canvas
                                        class="ff-canvas ff-canvas-ready"
                                        width="490" height="368">
                                    </canvas><img alt=""
                                        src="/e5ab717f39cfbb99638bad3b3e57b98e.gif"
                                        data-ff="true"
                                        class="ff-image">
                                </div>
                            </div>
```

Remove the `lab-congrats__body` div
```html
 <div class="lab-congrats__body">
                                <h3
                                    class="lab-heading lab-heading--medium-plus lab-heading-- lab-heading--big-space">
                                    <span>Congratulations on
                                        completing this lab!</span>
                                </h3>
                            </div>
```

Update the height and width of the `ant-modal` div to the following:
```html
<div role="document" class="ant-modal"
    style="top: 95px; width: 864px; height: 573px; transform-origin: -189px 841px;">
```

Change thumbs up / down SVGs to the following
Add the following arrow SVG before the button
```html
<svg width="9" height="16" viewBox="0 0 9 16" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 15L1 8L8 1" stroke="#1E557A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

```
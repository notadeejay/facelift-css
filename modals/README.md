## Congrats Modals

- Will need to `ps-logo-modal.png` image for the background of BOTH modals

## Lesson Modal

- Switch the clock SVG with the following:

```html
<svg width="15" height="15" viewBox="0 0 15 15" fill="none" xmlns="http://www.w3.org/2000/svg">
<circle cx="7.5" cy="7.5" r="7.5" fill="black"/>
<path d="M7 3.5V8.5L11 10" stroke="#C9EDFB" stroke-width="1.2"/>
</svg>

```

- Remove the Module Name and SVG that goes along with it.

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

**Thumbs Up**

```html
<svg width="25"
    height="24"
    viewBox="0 0 25 24"
    fill="none"
    xmlns="http://www.w3.org/2000/svg">
    <path
        d="M12.0156 3.07211C10.8561 6.92484 8.60134 8.74112 7.18408 9.25648V21.6252H18.5865C20.4418 21.6252 21.2922 19.8214 21.4855 18.9196C21.7431 17.6956 22.4131 14.4745 23.0316 11.3823C23.65 8.29015 21.3566 7.90363 20.1326 8.09689L13.9482 8.67668C14.528 8.0969 15.5166 6.28114 16.2674 4.03841C17.2337 1.15203 13.117 -0.587333 12.0156 3.07211Z"
        stroke="#039BE8"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round" />
    <rect x="1"
        y="7.52979"
        width="6.18438"
        height="15.461"
        stroke="#039BE8"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round" />
</svg>
```

**Thumbs Down**

```html
<svg
    width="25" height="25"
    viewBox="0 0 25 25"
    fill="none"
    xmlns="http://www.w3.org/2000/svg">
    <path
        d="M12.5315 21.6563C13.734 17.6609 16.0722 15.7773 17.542 15.2429L17.542 2.416L5.7172 2.416C3.79316 2.416 2.91131 4.28659 2.71089 5.22188C2.44367 6.49121 1.74888 9.83155 1.10753 13.0383C0.466185 16.245 2.84451 16.6458 4.11383 16.4454L10.5273 15.8442C9.92602 16.4454 8.90087 18.3284 8.12224 20.6542C7.12014 23.6475 11.3893 25.4513 12.5315 21.6563Z"
        stroke="#039BE8"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round" />
    <rect x="23.9551"
        y="17.0337"
        width="6.41345"
        height="16.0336"
        transform="rotate(-180 23.9551 17.0337)"
        stroke="#039BE8"
        stroke-width="2"
        stroke-linecap="round"
        stroke-linejoin="round" />
</svg>
```

Add the following arrow SVG to the `.congrats-form__link` button, before the `<span>`

```html
<svg width="9" height="16" viewBox="0 0 9 16" fill="none" xmlns="http://www.w3.org/2000/svg">
<path d="M8 15L1 8L8 1" stroke="#1E557A" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
</svg>

```
## Implementation Considerations 

- The general layout and responsiveness of the page should remain the same as it is now. This is not 100% reflected in the CSS right now. I've added media queries for particular items that required alternate layouts but did not include them for the general layout of the lesson page. 

### Lesson Part

- Removed the circle SVG from the Part Header

- Need to remove the animated green confetti / gifs from the Part Header and Footer on complete. TBD what animation might replace these.

### Lesson HTML Block
- Changed the H1s in the HTML blocks to --> H2s and added a class of `html__title`

```html
<div class="lesson-part__contentBlock">
    <div class="block html"
        name="block_98351726-b470-4c1e-9c09-6ace4c2167a7">
        <div class="section">
            <div class="html__title">
                <h2>This Block Includes Dropdowns
                </h2>
            </div>
            .....

```
### Collapsible Snippet Block

- Added negative margin so that it will appear like an accordion menu in relation to the previous block

### Knowledge Check Block

- Moved the `steps` to navigate between questions into to the `answer-buttons` div

```html
<div class="answer-buttons">
    <div class="steps"
        aria-labelledby="question-progress">
        <button
            type="button"
            disabled=""
            class="steps__arrow left disabled"
            aria-label="Previous">
            <svg width="16" height="28" viewBox="0 0 16 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M14 2L2 14L14 26" stroke-width="3" stroke-linejoin="round"/>
                </svg>
                
        </button>
        <button
            type="button"
            class="steps__arrow right"
            aria-label="Next">
            <svg width="16" height="28" viewBox="0 0 16 28" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M2 2L14 14L2 26"  stroke-width="3" stroke-linejoin="round"/>
                </svg>
                
        </button>
    </div>
    <div
        class="answer-buttons__buttons">
        <button
            type="button"
            class="button-standard button-standard--green button-standard--short"><span>Next</span></button>
    </div>
</div>
```

- Removed the SVG from the KC block label
- Moved the Instruction / Questions tabs into the `knowledge-check__header`

```html
<div
    class="knowledge-check__header">
    <h1 class="heading">
        Missing Values in
        the World
        Happiness Dataset
    </h1>

    <ul class="tabs"
        role="tablist">
        <li class="tabs__item"
            role="tab"
            id="react-tabs-4"
            aria-selected="true"
            aria-disabled="false"
            aria-controls="react-tabs-5"
            tabindex="0">
            <span>Instructions</span>
        </li>
        <li class="tabs__item tabs__item--active"
            role="tab"
            id="react-tabs-6"
            aria-selected="false"
            aria-disabled="false"
            aria-controls="react-tabs-7">
            <span>Questions
                (2)</span>
        </li>
    </ul>

</div>
```

- Removed the `div` around the input label

```html
      <div
        class="question">
        <input
            id="questions-b59793b7-97a0-4f3a-bef6-e2af1b615bf1-0-multiple"
            name="question-b59793b7-97a0-4f3a-bef6-e2af1b615bf1"
            type="checkbox">
         <!-- used to be a div here -->
        <label
            class="false"
            for="questions-b59793b7-97a0-4f3a-bef6-e2af1b615bf1-0-multiple">
            <p>The median is 21.5
            </p>
        </label>

    </div>
```



## Next.Tech, Embed, Typeform Block

- Changed `heading` to an H2

```html
<div class="lesson-part__contentBlock">
                        <div class="block embed"
                            name="block_23a892ff-1a0b-4fca-871c-a06a5bc217c1">
                            <div class="section">
                                <h2 class="heading">Google Sheet</h2>
                            </div>
                            ....
```

## Video

- Moved `H2` below the `iframe`

```html
 <div
    class="block-label__content">

    <div
        style="width: 100%;">
        <iframe
            width="100%"
            height="500"
            src="https://www.youtube.com/embed/aY6LiTbfckA"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen=""
            title="Salesforce Business Analyst Intro"></iframe>
    </div>
    <h2
        class="heading">
        How to Setup
        MySQL
        Workbench
    </h2>
```

- Switched label SVG to come before label

```html
<div
    class="block-header block-label__wrapper block-label__wrapper--static">
    <span
        class="block-icon icon-element icon-element--fill-transparent icon-element--background-transparent  icon-element--size-"><svg
            width="22"
            height="12"
            viewBox="0 0 22 16">
            <path
                d="M20.167 0c-.507 0-.917.398-.917.889 0 .49-.41.889-.917.889-.506 0-.916-.398-.916-.89 0-.49-.41-.888-.917-.888-.506 0-.917.398-.917.889 0 .49-.41.889-.916.889-.507 0-.917-.398-.917-.89 0-.49-.41-.888-.917-.888-.506 0-.916.398-.916.889 0 .49-.41.889-.917.889-.506 0-.917-.398-.917-.89 0-.49-.41-.888-.916-.888-.507 0-.917.398-.917.889 0 .49-.41.889-.917.889-.506 0-.916-.398-.916-.89C6.417.399 6.007 0 5.5 0c-.506 0-.917.398-.917.889 0 .49-.41.889-.916.889-.507 0-.917-.398-.917-.89C2.75.399 2.34 0 1.833 0 .821 0 0 .796 0 1.778v12.444C0 15.204.82 16 1.833 16c.507 0 .917-.398.917-.889 0-.49.41-.889.917-.889.506 0 .916.398.916.89 0 .49.41.888.917.888.506 0 .917-.398.917-.889 0-.49.41-.889.916-.889.507 0 .917.398.917.89 0 .49.41.888.917.888.506 0 .916-.398.916-.889 0-.49.41-.889.917-.889.506 0 .917.398.917.89 0 .49.41.888.916.888.507 0 .917-.398.917-.889 0-.49.41-.889.917-.889.506 0 .916.398.916.89 0 .49.41.888.917.888.506 0 .917-.398.917-.889 0-.49.41-.889.916-.889.507 0 .917.398.917.89 0 .49.41.888.917.888C21.179 16 22 15.204 22 14.222V1.778C22 .796 21.18 0 20.167 0zm-5.83 8.756L9.653 11.6a.941.941 0 01-.932.023.885.885 0 01-.471-.779v-5.68c0-.323.18-.621.471-.778a.941.941 0 01.932.023l4.684 2.844a.883.883 0 01.426.751c0 .305-.16.589-.426.752z"
                fill="#1E557A"
                fill-rule="evenodd">
            </path>
        </svg></span>
    <span
        class="label"><span>Media</span></span>
</div>
```

### Lab Block

- Moved the block label SVG to before the label span

```html
<div
    class="block-header block-label__wrapper block-label__wrapper--static">
    <span
        class="block-icon icon-element icon-element--fill-transparent icon-element--background-transparent  icon-element--size-">
        <svg width="14"
            height="16"
            viewBox="0 0 14 16"
            fill="none"
            xmlns="http://www.w3.org/2000/svg">
            <path
                d="M12.7176 11.6372L10.5696 8.39348H3.42846L1.28053 11.6372C1.04505 11.9927 0.919243 12.3814 0.906052 12.793C0.893838 13.1771 0.983488 13.5634 1.16499 13.9102C1.34673 14.257 1.61201 14.5482 1.93226 14.7523C2.27547 14.971 2.66338 15.082 3.085 15.082H10.9131C11.3347 15.082 11.7226 14.971 12.0658 14.7523C12.3861 14.5482 12.6514 14.257 12.8331 13.9102C13.0149 13.5634 13.1043 13.1771 13.0921 12.793C13.0791 12.3814 12.9531 11.9927 12.7176 11.6372ZM4.15909 12.5259C3.85643 12.5259 3.61117 12.2767 3.61117 11.9691C3.61117 11.6615 3.85643 11.4123 4.15909 11.4123C4.46175 11.4123 4.707 11.6615 4.707 11.9691C4.707 12.2767 4.46175 12.5259 4.15909 12.5259ZM5.46035 10.3683C5.46035 10.1568 5.6289 9.98554 5.83703 9.98554C6.04515 9.98554 6.2137 10.1568 6.2137 10.3683C6.2137 10.5799 6.04515 10.7512 5.83703 10.7512C5.6289 10.7512 5.46035 10.5799 5.46035 10.3683ZM6.00802 13.2915C5.7999 13.2915 5.63135 13.1202 5.63135 12.9087C5.63135 12.6972 5.7999 12.5259 6.00802 12.5259C6.21614 12.5259 6.3847 12.6972 6.3847 12.9087C6.3847 13.12 6.21614 13.2915 6.00802 13.2915ZM13.467 11.1245L9.88103 5.70936C9.6883 5.4184 9.58643 5.07904 9.58643 4.72825V0.65564H9.83828C10.0161 0.65564 10.161 0.508673 10.161 0.327696C10.161 0.146967 10.0164 0 9.83853 0H4.15958C3.98174 0 3.83689 0.146967 3.83689 0.327944C3.83689 0.508673 3.9815 0.655888 4.15958 0.655888H4.41143V4.7285C4.41143 5.07929 4.30956 5.41865 4.11683 5.7096L0.531087 11.1245C-0.11527 12.1004 -0.176339 13.3032 0.367665 14.3414C0.91167 15.3799 1.92737 15.9998 3.085 15.9998H10.9131C12.0707 15.9998 13.0864 15.3799 13.6304 14.3414C14.1744 13.3032 14.1134 12.1007 13.467 11.1245ZM13.0608 14.0336C12.858 14.4209 12.5612 14.7463 12.2026 14.9747C11.8177 15.22 11.3838 15.3444 10.9129 15.3444H3.085C2.61404 15.3444 2.1802 15.22 1.79522 14.9747C1.43687 14.7463 1.14007 14.4209 0.937075 14.0336C0.734325 13.6463 0.634172 13.2146 0.647851 12.7846C0.662508 12.3231 0.803211 11.8877 1.06605 11.4907L3.65368 7.58318H5.24026C5.41809 7.58318 5.56295 7.43621 5.56295 7.25524C5.56295 7.07451 5.41834 6.92729 5.24026 6.92729H4.08825L4.65228 6.07553C4.84062 5.79128 4.96447 5.47848 5.02139 5.14383H6.37273C6.55056 5.14383 6.69542 4.99687 6.69542 4.81589C6.69542 4.63516 6.5508 4.48794 6.37273 4.48794H5.05681V2.70448H6.37273C6.55056 2.70448 6.69542 2.55752 6.69542 2.37654C6.69542 2.19556 6.5508 2.0486 6.37273 2.0486H5.05681V0.65564H8.9413V4.72825C8.9413 5.20987 9.08127 5.67584 9.34582 6.07553L12.9318 11.4907C13.1946 11.8877 13.3354 12.3231 13.3503 12.7846C13.3637 13.2143 13.2638 13.6463 13.0608 14.0336Z"
                fill="white" />
        </svg>

    </span><span
        class="label"><span>Lab</span></span>
</div>
```

- Added a `launch__wrapper` around the `launch` button, and added an SVG graphic
```html
<div class="launch__wrapper">
    <svg width="231" height="138" viewBox="0 0 231 138" fill="none" xmlns="http://www.w3.org/2000/svg">
        <g filter="url(#filter0_d)">
        <rect x="7" y="7.30579" width="216" height="122.293" fill="#154268"/>
        </g>
        <path d="M16 72.2739H135" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M16 79.9172H135" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M16 87.5605H135" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M16 56.9873H135" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M16 64.6306H135" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M88 47.4331L88 98.0701" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M112 47.4331L112 98.0701" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M64 47.4331L64 98.0701" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M40 47.4331L40 98.0701" stroke="#5EB3EA" stroke-width="0.5"/>
        <path d="M2 27.3694L2 1.5732L34 1.57321" stroke="#039BE8" stroke-width="3"/>
        <path d="M228.7 109.726V135.522H196.7" stroke="#039BE8" stroke-width="3"/>
        <rect x="16.25" y="49.594" width="118.5" height="45.3599" stroke="#368FD5" stroke-width="0.5"/>
        <path d="M16 26.4141L213 26.4141" stroke="#5EB3EA"/>
        <path d="M213 63.6752L122 63.6752" stroke="#039BE8" stroke-width="3" stroke-dasharray="3 16"/>
        <path d="M213 77.0509L122 77.0509" stroke="#039BE8" stroke-width="3" stroke-dasharray="3 16"/>
        <path d="M213 90.4268L122 90.4268" stroke="#039BE8" stroke-width="3" stroke-dasharray="3 16"/>
        <path d="M213 103.802L122 103.802" stroke="#039BE8" stroke-width="3" stroke-dasharray="3 16"/>
        <path d="M213 117.178L122 117.178" stroke="#039BE8" stroke-width="3" stroke-dasharray="3 16"/>
        <ellipse cx="19.5" cy="17.3376" rx="2.5" ry="2.38854" fill="#0278C7"/>
        <ellipse cx="29.5" cy="17.3376" rx="2.5" ry="2.38854" fill="#368FD5"/>
        <ellipse cx="39.5" cy="17.3376" rx="2.5" ry="2.38854" fill="#5EB3EA"/>
        <rect x="151.3" y="16.2044" width="60.4" height="2.26624" fill="#039BE8" stroke="#039BE8" stroke-width="0.6"/>
        <path d="M64.4464 111.751C62.6056 111.242 61.0422 109.964 60.3208 108.15C59.0844 105.042 60.7906 101.539 64.1318 100.326C67.4729 99.1123 71.1838 100.649 72.4203 103.757C73.1694 105.64 72.8384 107.668 71.7182 109.244" stroke="white" stroke-width="1.5" stroke-linecap="round"/>
        <path d="M74.3274 110.353C75.9134 108.002 76.3205 105.033 75.1442 102.33C73.2026 97.8665 67.6823 95.8155 62.8143 97.7487C57.9463 99.6818 55.574 104.867 57.5156 109.33C58.5598 111.73 60.639 113.433 63.0952 114.193" stroke="white" stroke-linecap="round"/>
        <path d="M64.7528 132.296L64.8916 104.459L86.1571 123.264L78.6614 124.686L83.0424 134.162L76.2062 137.047L71.8253 127.57L64.7528 132.296Z" fill="#154268" stroke="#368FD5" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
        <defs>
        <filter id="filter0_d" x="3" y="7.30579" width="224" height="130.293" filterUnits="userSpaceOnUse" color-interpolation-filters="sRGB">
        <feFlood flood-opacity="0" result="BackgroundImageFix"/>
        <feColorMatrix in="SourceAlpha" type="matrix" values="0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 127 0"/>
        <feOffset dy="4"/>
        <feGaussianBlur stdDeviation="2"/>
        <feColorMatrix type="matrix" values="0 0 0 0 0.117647 0 0 0 0 0.333333 0 0 0 0 0.478431 0 0 0 0.15 0"/>
        <feBlend mode="normal" in2="BackgroundImageFix" result="effect1_dropShadow"/>
        <feBlend mode="normal" in="SourceGraphic" in2="effect1_dropShadow" result="shape"/>
        </filter>
        </defs>
        </svg>
        
<button
    type="button"
    class="launch"><span>Launch
        Lab</span></button>
    </div>
```

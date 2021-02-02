## Implementation Considerations

- Need to change the SVG for the back button. It is included in `lab-sidebar.html`
- Need to move the Download Files button to directly below the  `lab-exercise__header`. The following code contains an updated class name and a new SVG

```html
<div class="lab-exercise__download">
    <div
        class="authoring-dropdown full-width small-list">
        <button
            class="button-standard button-standard--grey button-standard--transparent"
            type="button"><span>Download
                files</span><svg width="16" height="9" viewBox="0 0 16 9" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M15 1L8 8L0.999999 1" stroke="#1E557A" stroke-width="1.5" stroke-linecap="round" stroke-linejoin="round"/>
                    </svg>
                    </button>
        <div class="collapsible"><button
                type="button"><span>Download db
                    starter
                    file</span></button><button
                type="button"><span>Download query
                    starter file</span></button>
        </div>
    </div>
</div> 
```
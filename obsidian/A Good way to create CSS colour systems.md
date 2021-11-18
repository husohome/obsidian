# How to Create themes css
#web #coding #css

This! source: obsidian themes
1. create define base colours in `:root`
2. create a `.theme` class and define a few colours you need: bg-primary, ..., text-title-h1, ..., you get the idea, and use `var(--red)`
```
:root
{
    --dark0:  #2e3440;
    --dark1:  #3b4252;
    --dark2:  #434c5e;
    --dark3:  #4c566a;

    --light0: #d8dee9;
    --light1: #e5e9f0;
    --light2: #eceff4;
    --light3: #ffffff;

    --frost0: #8fbcbb;
    --frost1: #88c0d0;
    --frost2: #81a1c1;
    --frost3: #5e81ac;

    --red:    #bf616a;
    --orange: #d08770;
    --yellow: #ebcb8b;
    --green:  #a3be8c;
    --purple: #b48ead;
}

.theme-dark
{
    --background-primary:         var(--dark0);
    --background-primary-alt:     var(--dark0);
    --background-secondary:       var(--dark1);
    --background-secondary-alt:   var(--dark2);
    --text-normal:                var(--light2);
    --text-faint:                 var(--light0);
    --text-muted:                 var(--light1);
    --text-title-h1:              var(--green);
    --text-title-h2:              var(--yellow);
    --text-title-h3:              var(--blue);
    --text-title-h4:              var(--green);
    --text-title-h5:              var(--purple);
    --text-title-h6:              var(--orange);
    --text-link:                  var(--frost0);
    --text-a:                     var(--frost3);
    --text-a-hover:               var(--frost2);
    --text-mark:                  rgba(136, 192, 208, 0.3); /* frost1 */
    --pre-code:                   var(--dark1);
    --text-highlight-bg:          var(--red);
    --text-highlight-bg-active:   var(--green);
    --interactive-accent:         var(--frost0);
    --interactive-before:         var(--dark3);
    --background-modifier-border: var(--dark2);
    --text-accent:                var(--orange);
    --interactive-accent-rgb:     var(--orange);
    --inline-code:                var(--frost1);
    --code-block:                 var(--frost1);
    --vim-cursor:                 var(--orange);
    --text-selection:             var(--dark3);
    --text-tag:                   var(--frost0);
    --task-checkbox:              var(--frost0);
}
.theme-light
{
	--background-primary:         var(--light3);
	--background-primary-alt:     var(--light3);
	--background-secondary:       var(--light2);
	--background-secondary-alt:   var(--light1);
	--text-normal:                var(--dark1);
	--text-faint:                 var(--dark3);
	--text-muted:                 var(--dark2);
	--text-title-h1:              var(--red);
	--text-title-h2:              var(--orange);
	--text-title-h3:              var(--yellow);
	--text-title-h4:              var(--green);
	--text-title-h5:              var(--purple);
	--text-title-h6:              var(--orange);
	--text-link:                  var(--frost0);
	--text-a:                     var(--frost3);
	--text-a-hover:               var(--frost1);
	--text-mark:                  rgba(136, 192, 208, 0.3); /* frost1 */
	--pre-code:                   var(--light2);
	--text-highlight-bg:          var(--green);
    --text-highlight-bg-active:   var(--yellow);
	--interactive-accent:         var(--frost0);
	--interactive-before:         var(--light0);
	--background-modifier-border: var(--light1);
	--text-accent:                var(--orange);
	--interactive-accent-rgb:     var(--orange);
	--inline-code:                var(--frost1);
	--code-block:                 var(--frost1);
	--vim-cursor:                 var(--orange);
	--text-selection:             var(--light0);
    --text-tag:                   var(--frost2);
    --task-checkbox:              var(--frost0);
}
```
/*!
 * Default theme for Pingendo 
 * Homepage: http://pingendo.com  
 * Copyright 2015 Pingendo 
 * Licensed under MIT 
 * Based on Bootstrap v3.3.4
*/


/* Add custom CSS classes here 
 * 
 * img {
 *   box-shadow : 0px 0px 10px black !important;
 * }
*/

//
// Variables
// --------------------------------------------------
//== Colors
//
//## Gray and brand colors for use across Bootstrap.
@gray-base : #000;
@gray-darker : lighten(@gray-base, 13.5%); // #222
@gray-dark : lighten(@gray-base, 20%); // #333
@gray : lighten(@gray-base, 33.5%); // #555
@gray-light : lighten(@gray-base, 46.7%); // #777
@gray-lighter : lighten(@gray-base, 93.5%); // #eee
@brand-primary : #337CBB;
@brand-success : #5cb85c;
@brand-info : #5bc0de;
@brand-warning : #f0ad4e;
@brand-danger : #d9534f;
//== Scaffolding
//
//## Settings for some of the most global styles.
//** Background color for `<body>`.
@body-bg : white;
//** Global text color on `<body>`.
@text-color : black;
//** Global textual link color.
@link-color : @brand-primary;
//** Link hover color set via `darken()` function.
@link-hover-color : darken(@link-color, 15%);
//** Link hover decoration.
@link-hover-decoration : underline;
//== Typography
//
//## Font, line-height, and color for body text, headings, and more.
@font-family-sans-serif : "Helvetica Neue",
Helvetica,
Arial,
sans-serif;
@font-family-serif : Georgia,
"Times New Roman",
Times,
serif;
//** Default monospace fonts for `<code>`, `<kbd>`, and `<pre>`.
@font-family-monospace : Menlo,
Monaco,
Consolas,
"Courier New",
monospace;
@font-family-base : Lato;
@font-size-base : 14px;
@font-size-large : ceil((@font-size-base * 1.25)); // ~18px
@font-size-small : ceil((@font-size-base * 0.85)); // ~12px
@font-size-h1 : floor((@font-size-base * 2.6)); // ~36px
@font-size-h2 : floor((@font-size-base * 2.15)); // ~30px
@font-size-h3 : ceil((@font-size-base * 1.7)); // ~24px
@font-size-h4 : ceil((@font-size-base * 1.25)); // ~18px
@font-size-h5 : @font-size-base;
@font-size-h6 : ceil((@font-size-base * 0.85)); // ~12px
//** Unit-less `line-height` for use in components like buttons.
@line-height-base : 1.428571429; // 20/14
//** Computed "line-height" (`font-size` * `line-height`) for use with `margin`, `padding`, etc.
@line-height-computed : floor((@font-size-base * @line-height-base)); // ~20px
//** By default, this inherits from the `<body>`.
@headings-font-family : Lato;
@headings-font-weight : 500;
@headings-line-height : 1.1;
@headings-color : inherit;
//== Iconography
//
//## Specify custom location and filename of the included Glyphicons icon font. Useful for those including Bootstrap via Bower.
//** Load fonts from this directory.
@icon-font-path : "../fonts/";
//** File name for all font files.
@icon-font-name : "glyphicons-halflings-regular";
//** Element ID within SVG icon file.
@icon-font-svg-id : "glyphicons_halflingsregular";
//== Components
//
//## Define common padding and border radius sizes and more. Values based on 14px text and 1.428 line-height (~20px to start).
@padding-base-vertical : 6px;
@padding-base-horizontal : 12px;
@padding-large-vertical : 10px;
@padding-large-horizontal : 16px;
@padding-small-vertical : 5px;
@padding-small-horizontal : 10px;
@padding-xs-vertical : 1px;
@padding-xs-horizontal : 5px;
@line-height-large : 1.3333333; // extra decimals for Win 8.1 Chrome
@line-height-small : 1.5;
@border-radius-base : 4px;
@border-radius-large : 6px;
@border-radius-small : 3px;
//** Global color for active items (e.g., navs or dropdowns).
@component-active-color : contrast(@component-active-bg, @text-color, @text-inverse, 43%);
//** Global background color for active items (e.g., navs or dropdowns).
@component-active-bg : @brand-primary;
//** Width of the `border` for generating carets that indicator dropdowns.
@caret-width-base : 4px;
//** Carets increase slightly in size for larger components.
@caret-width-large : 5px;
//== Tables
//
//## Customizes the `.table` component with basic values, each used across all table variations.
//** Padding for `<th>`s and `<td>`s.
@table-cell-padding : 8px;
//** Padding for cells in `.table-condensed`.
@table-condensed-cell-padding : 5px;
//** Default background color used for all tables.
@table-bg : transparent;
//** Background color used for `.table-striped`.
@table-bg-accent : #f9f9f9;
//** Background color used for `.table-hover`.
@table-bg-hover : #f5f5f5;
@table-bg-active : @table-bg-hover;
//** Border color for table and cell borders.
@table-border-color : #ddd;
//== Buttons
//
//## For each of Bootstrap's buttons, define text, background and border color.
@btn-font-weight : normal;
@btn-default-color : @text-color;
@btn-default-bg : @body-bg;
@btn-default-border : #ccc;
@btn-primary-color : white;
@btn-primary-bg : @brand-primary;
@btn-primary-border : darken(@btn-primary-bg, 5%);
@btn-success-color : white;
@btn-success-bg : @brand-success;
@btn-success-border : darken(@btn-success-bg, 5%);
@btn-info-color : white;
@btn-info-bg : @brand-info;
@btn-info-border : darken(@btn-info-bg, 5%);
@btn-warning-color : white;
@btn-warning-bg : @brand-warning;
@btn-warning-border : darken(@btn-warning-bg, 5%);
@btn-danger-color : contrast(@btn-danger-bg, @text-color, @text-inverse, 43%);
@btn-danger-bg : @brand-danger;
@btn-danger-border : darken(@btn-danger-bg, 5%);
@btn-link-disabled-color : @gray-light;
//== Forms
//
//##
//** `<input>` background color
@input-bg : #fff;
//** `<input disabled>` background color
@input-bg-disabled : @gray-lighter;
//** Text color for `<input>`s
@input-color : @gray;
//** `<input>` border color
@input-border : #ccc;
// TODO: Rename `@input-border-radius` to `@input-border-radius-base` in v4
//** Default `.form-control` border radius
@input-border-radius : @border-radius-base;
//** Large `.form-control` border radius
@input-border-radius-large : @border-radius-large;
//** Small `.form-control` border radius
@input-border-radius-small : @border-radius-small;
//** Border color for inputs on focus
@input-border-focus : #66afe9;
//** Placeholder text color
@input-color-placeholder : #999;
//** Default `.form-control` height
@input-height-base : (@line-height-computed + (@padding-base-vertical * 2) + 2);
//** Large `.form-control` height
@input-height-large : (ceil(@font-size-large * @line-height-large) + (@padding-large-vertical * 2) + 2);
//** Small `.form-control` height
@input-height-small : (floor(@font-size-small * @line-height-small) + (@padding-small-vertical * 2) + 2);
//** `.form-group` margin
@form-group-margin-bottom: 15px;
@legend-color : @gray-dark;
@legend-border-color : #e5e5e5;
//** Background color for textual input addons
@input-group-addon-bg : @gray-lighter;
//** Border color for textual input addons
@input-group-addon-border-color : @input-border;
//** Disabled cursor for form controls and buttons.
@cursor-disabled : not-allowed;
//== Dropdowns
//
//## Dropdown menu container and contents.
//** Background for the dropdown menu.
@dropdown-bg : #fff;
//** Dropdown menu `border-color`.
@dropdown-border : rgba(0, 0, 0, .15);
//** Dropdown menu `border-color` **for IE8**.
@dropdown-fallback-border : #ccc;
//** Divider color for between dropdown items.
@dropdown-divider-bg : #e5e5e5;
//** Dropdown link text color.
@dropdown-link-color : @gray-dark;
//** Hover color for dropdown links.
@dropdown-link-hover-color : darken(@gray-dark, 5%);
//** Hover background for dropdown links.
@dropdown-link-hover-bg : #f5f5f5;
//** Active dropdown menu item text color.
@dropdown-link-active-color : @component-active-color;
//** Active dropdown menu item background color.
@dropdown-link-active-bg : @component-active-bg;
//** Disabled dropdown menu item background color.
@dropdown-link-disabled-color : @gray-light;
//** Text color for headers within dropdown menus.
@dropdown-header-color : @gray-light;
//** Deprecated `@dropdown-caret-color` as of v3.1.0
@dropdown-caret-color : #000;
//-- Z-index master list
//
// Warning: Avoid customizing these values. They're used for a bird's eye view
// of components dependent on the z-axis and are designed to all work together.
//
// Note: These variables are not generated into the Customizer.
@zindex-navbar : 1000;
@zindex-dropdown : 1000;
@zindex-popover : 1060;
@zindex-tooltip : 1070;
@zindex-navbar-fixed : 1030;
@zindex-modal-background: 1040;
@zindex-modal: 1050;
//== Media queries breakpoints
//
//## Define the breakpoints at which your layout will change, adapting to different screen sizes.
// Extra small screen / phone
//** Deprecated `@screen-xs` as of v3.0.1
@screen-xs : 480px;
//** Deprecated `@screen-xs-min` as of v3.2.0
@screen-xs-min : @screen-xs;
//** Deprecated `@screen-phone` as of v3.0.1
@screen-phone : @screen-xs-min;
// Small screen / tablet
//** Deprecated `@screen-sm` as of v3.0.1
@screen-sm : 768px;
@screen-sm-min : @screen-sm;
//** Deprecated `@screen-tablet` as of v3.0.1
@screen-tablet : @screen-sm-min;
// Medium screen / desktop
//** Deprecated `@screen-md` as of v3.0.1
@screen-md : 992px;
@screen-md-min : @screen-md;
//** Deprecated `@screen-desktop` as of v3.0.1
@screen-desktop : @screen-md-min;
// Large screen / wide desktop
//** Deprecated `@screen-lg` as of v3.0.1
@screen-lg : 1200px;
@screen-lg-min : @screen-lg;
//** Deprecated `@screen-lg-desktop` as of v3.0.1
@screen-lg-desktop : @screen-lg-min;
// So media queries don't overlap when required, provide a maximum
@screen-xs-max : (@screen-sm-min - 1);
@screen-sm-max : (@screen-md-min - 1);
@screen-md-max : (@screen-lg-min - 1);
//== Grid system
//
//## Define your custom responsive grid.
//** Number of columns in the grid.
@grid-columns : 12;
//** Padding between columns. Gets divided in half for the left and right.
@grid-gutter-width : 30px;
// Navbar collapse
//** Point at which the navbar becomes uncollapsed.
@grid-float-breakpoint : @screen-sm-min;
//** Point at which the navbar begins collapsing.
@grid-float-breakpoint-max : (@grid-float-breakpoint - 1);
//== Container sizes
//
//## Define the maximum width of `.container` for different screen sizes.
// Small screen / tablet
@container-tablet : (720px + @grid-gutter-width);
//** For `@screen-sm-min` and up.
@container-sm : @container-tablet;
// Medium screen / desktop
@container-desktop : (940px + @grid-gutter-width);
//** For `@screen-md-min` and up.
@container-md : @container-desktop;
// Large screen / wide desktop
@container-large-desktop : (1140px + @grid-gutter-width);
//** For `@screen-lg-min` and up.
@container-lg : @container-large-desktop;
//== Navbar
//
//##
// Basics of a navbar
@navbar-height : 50px;
@navbar-margin-bottom : @line-height-computed;
@navbar-border-radius : @border-radius-base;
@navbar-padding-horizontal : floor((@grid-gutter-width / 2));
@navbar-padding-vertical : ((@navbar-height - @line-height-computed) / 2);
@navbar-collapse-max-height : 340px;
@navbar-default-color : black;
@navbar-default-bg : #f8f8f8;
@navbar-default-border : darken(@navbar-default-bg, 6.5%);
// Navbar links
@navbar-default-link-color : contrast(@navbar-default-bg, @text-color, @text-inverse, 43%);
@navbar-default-link-hover-color : @navbar-default-color;
@navbar-default-link-hover-bg : transparent;
@navbar-default-link-active-color : @navbar-default-color;
@navbar-default-link-active-bg : darken(@navbar-default-bg, 6.5%);
@navbar-default-link-disabled-color : #ccc;
@navbar-default-link-disabled-bg : transparent;
// Navbar brand label
@navbar-default-brand-color : @navbar-default-link-color;
@navbar-default-brand-hover-color : darken(@navbar-default-brand-color, 10%);
@navbar-default-brand-hover-bg : transparent;
// Navbar toggle
@navbar-default-toggle-hover-bg : #ddd;
@navbar-default-toggle-icon-bar-bg : #888;
@navbar-default-toggle-border-color : #ddd;
// Inverted navbar
// Reset inverted navbar basics
@navbar-inverse-color : lighten(@gray-light, 15%);
@navbar-inverse-bg : #222;
@navbar-inverse-border : darken(@navbar-inverse-bg, 10%);
// Inverted navbar links
@navbar-inverse-link-color : lighten(@gray-light, 15%);
@navbar-inverse-link-hover-color : #fff;
@navbar-inverse-link-hover-bg : transparent;
@navbar-inverse-link-active-color : @navbar-inverse-link-hover-color;
@navbar-inverse-link-active-bg : darken(@navbar-inverse-bg, 10%);
@navbar-inverse-link-disabled-color : #444;
@navbar-inverse-link-disabled-bg : transparent;
// Inverted navbar brand label
@navbar-inverse-brand-color : @navbar-inverse-link-color;
@navbar-inverse-brand-hover-color : #fff;
@navbar-inverse-brand-hover-bg : transparent;
// Inverted navbar toggle
@navbar-inverse-toggle-hover-bg : #333;
@navbar-inverse-toggle-icon-bar-bg : #fff;
@navbar-inverse-toggle-border-color : #333;
//== Navs
//
//##
//=== Shared nav styles
@nav-link-padding : 10px 15px;
@nav-link-hover-bg : @gray-lighter;
@nav-disabled-link-color : @gray-light;
@nav-disabled-link-hover-color : @gray-light;
//== Tabs
@nav-tabs-border-color : #ddd;
@nav-tabs-link-hover-border-color : @gray-lighter;
@nav-tabs-active-link-hover-bg : @body-bg;
@nav-tabs-active-link-hover-color : @gray;
@nav-tabs-active-link-hover-border-color : #ddd;
@nav-tabs-justified-link-border-color : #ddd;
@nav-tabs-justified-active-link-border-color : @body-bg;
//== Pills
@nav-pills-border-radius : @border-radius-base;
@nav-pills-active-link-hover-bg : @component-active-bg;
@nav-pills-active-link-hover-color : @component-active-color;
//== Pagination
//
//##
@pagination-color : @link-color;
@pagination-bg : #fff;
@pagination-border : #ddd;
@pagination-hover-color : @link-hover-color;
@pagination-hover-bg : @gray-lighter;
@pagination-hover-border : #ddd;
@pagination-active-color : #fff;
@pagination-active-bg : @brand-primary;
@pagination-active-border : @brand-primary;
@pagination-disabled-color : @gray-light;
@pagination-disabled-bg : #fff;
@pagination-disabled-border : #ddd;
//== Pager
//
//##
@pager-bg : @pagination-bg;
@pager-border : @pagination-border;
@pager-border-radius : 15px;
@pager-hover-bg : @pagination-hover-bg;
@pager-active-bg : @pagination-active-bg;
@pager-active-color : @pagination-active-color;
@pager-disabled-color : @pagination-disabled-color;
//== Jumbotron
//
//##
@jumbotron-padding : 30px;
@jumbotron-color : inherit;
@jumbotron-bg : @gray-lighter;
@jumbotron-heading-color : inherit;
@jumbotron-font-size : ceil((@font-size-base * 1.5));
@jumbotron-heading-font-size: ceil((@font-size-base * 4.5));
//== Form states and alerts
//
//## Define colors for form feedback states and, by default, alerts.
@state-success-text : @brand-success;
@state-success-bg : lighten(@brand-success, 20%);
@state-success-border : darken(spin(@state-success-bg, -10), 5%);
@state-info-text : @brand-info;
@state-info-bg : lighten(@brand-info, 20%);
@state-info-border : darken(spin(@state-info-bg, -10), 7%);
@state-warning-text : @brand-warning;
@state-warning-bg : lighten(@brand-warning, 20%);
@state-warning-border : darken(spin(@state-warning-bg, -10), 5%);
@state-danger-text : @brand-danger;
@state-danger-bg : lighten(@brand-danger, 20%);
@state-danger-border : darken(spin(@state-danger-bg, -10), 5%);
//== Tooltips
//
//##
//** Tooltip max width
@tooltip-max-width : 200px;
//** Tooltip text color
@tooltip-color : #fff;
//** Tooltip background color
@tooltip-bg : #000;
@tooltip-opacity : .9;
//** Tooltip arrow width
@tooltip-arrow-width : 5px;
//** Tooltip arrow color
@tooltip-arrow-color : @tooltip-bg;
//== Popovers
//
//##
//** Popover body background color
@popover-bg : #fff;
//** Popover maximum width
@popover-max-width : 276px;
//** Popover border color
@popover-border-color : rgba(0, 0, 0, .2);
//** Popover fallback border color
@popover-fallback-border-color : #ccc;
//** Popover title background color
@popover-title-bg : darken(@popover-bg, 3%);
//** Popover arrow width
@popover-arrow-width : 10px;
//** Popover arrow color
@popover-arrow-color : @popover-bg;
//** Popover outer arrow width
@popover-arrow-outer-width : (@popover-arrow-width + 1);
//** Popover outer arrow color
@popover-arrow-outer-color : fadein(@popover-border-color, 5%);
//** Popover outer arrow fallback color
@popover-arrow-outer-fallback-color : darken(@popover-fallback-border-color, 20%);
//== Labels
//
//##
//** Default label background color
@label-default-bg : @gray-light;
//** Primary label background color
@label-primary-bg : @brand-primary;
//** Success label background color
@label-success-bg : @brand-success;
//** Info label background color
@label-info-bg : @brand-info;
//** Warning label background color
@label-warning-bg : @brand-warning;
//** Danger label background color
@label-danger-bg : @brand-danger;
//** Default label text color
@label-color : #fff;
//** Default text color of a linked label
@label-link-hover-color : #fff;
//== Modals
//
//##
//** Padding applied to the modal body
@modal-inner-padding : 15px;
//** Padding applied to the modal title
@modal-title-padding : 15px;
//** Modal title line-height
@modal-title-line-height : @line-height-base;
//** Background color of modal content area
@modal-content-bg : #fff;
//** Modal content border color
@modal-content-border-color : rgba(0, 0, 0, .2);
//** Modal content border color **for IE8**
@modal-content-fallback-border-color : #999;
//** Modal backdrop background color
@modal-backdrop-bg : #000;
//** Modal backdrop opacity
@modal-backdrop-opacity : .5;
//** Modal header border color
@modal-header-border-color : #e5e5e5;
//** Modal footer border color
@modal-footer-border-color : @modal-header-border-color;
@modal-lg : 900px;
@modal-md : 600px;
@modal-sm : 300px;
//== Alerts
//
//## Define alert colors, border radius, and padding.
@alert-padding : 15px;
@alert-border-radius : @border-radius-base;
@alert-link-font-weight : bold;
@alert-success-bg : @state-success-bg;
@alert-success-text : @state-success-text;
@alert-success-border : @state-success-border;
@alert-info-bg : @state-info-bg;
@alert-info-text : @state-info-text;
@alert-info-border : @state-info-border;
@alert-warning-bg : @state-warning-bg;
@alert-warning-text : @state-warning-text;
@alert-warning-border : @state-warning-border;
@alert-danger-bg : @state-danger-bg;
@alert-danger-text : @state-danger-text;
@alert-danger-border : @state-danger-border;
//== Progress bars
//
//##
//** Background color of the whole progress component
@progress-bg : #f5f5f5;
//** Progress bar text color
@progress-bar-color : #fff;
//** Variable for setting rounded corners on progress bar.
@progress-border-radius : @border-radius-base;
//** Default progress bar color
@progress-bar-bg : @brand-primary;
//** Success progress bar color
@progress-bar-success-bg : @brand-success;
//** Warning progress bar color
@progress-bar-warning-bg : @brand-warning;
//** Danger progress bar color
@progress-bar-danger-bg : @brand-danger;
//** Info progress bar color
@progress-bar-info-bg : @brand-info;
//== List group
//
//##
//** Background color on `.list-group-item`
@list-group-bg : @body-bg;
//** `.list-group-item` border color
@list-group-border : darken(@list-group-bg, 40%);
//** List group border radius
@list-group-border-radius : @border-radius-base;
//** Background color of single list items on hover
@list-group-hover-bg : #f5f5f5;
//** Text color of active list items
@list-group-active-color : @component-active-color;
//** Background color of active list items
@list-group-active-bg : @component-active-bg;
//** Border color of active list elements
@list-group-active-border : @list-group-active-bg;
//** Text color for content within active list items
@list-group-active-text-color : darken(@list-group-active-bg, 40%);
//** Text color of disabled list items
@list-group-disabled-color : @gray-light;
//** Background color of disabled list items
@list-group-disabled-bg : @gray-lighter;
//** Text color for content within disabled list items
@list-group-disabled-text-color : @list-group-disabled-color;
@list-group-link-color : #555;
@list-group-link-hover-color : @list-group-link-color;
@list-group-link-heading-color : #333;
//== Panels
//
//##
@panel-bg : @body-bg;
@panel-body-padding : 15px;
@panel-heading-padding : 10px 15px;
@panel-footer-padding : @panel-heading-padding;
@panel-border-radius : @border-radius-base;
//** Border color for elements within panels
@panel-inner-border : #ddd;
@panel-footer-bg : #f5f5f5;
@panel-default-text : @gray-dark;
@panel-default-border : #ddd;
@panel-default-heading-bg : #f5f5f5;
@panel-primary-text : contrast(@brand-primary, @text-color, @text-inverse, 43%);
@panel-primary-border : @brand-primary;
@panel-primary-heading-bg : @brand-primary;
@panel-success-text : @state-success-text;
@panel-success-border : @state-success-border;
@panel-success-heading-bg : @state-success-bg;
@panel-info-text : @state-info-text;
@panel-info-border : @state-info-border;
@panel-info-heading-bg : @state-info-bg;
@panel-warning-text : @state-warning-text;
@panel-warning-border : @state-warning-border;
@panel-warning-heading-bg : @state-warning-bg;
@panel-danger-text : @state-danger-text;
@panel-danger-border : @state-danger-border;
@panel-danger-heading-bg : @state-danger-bg;
//== Thumbnails
//
//##
//** Padding around the thumbnail image
@thumbnail-padding : 4px;
//** Thumbnail background color
@thumbnail-bg : @body-bg;
//** Thumbnail border color
@thumbnail-border : #ddd;
//** Thumbnail border radius
@thumbnail-border-radius : @border-radius-base;
//** Custom text color for thumbnail captions
@thumbnail-caption-color : @text-color;
//** Padding around the thumbnail caption
@thumbnail-caption-padding : 9px;
//== Wells
//
//##
@well-bg : #f5f5f5;
@well-border : darken(@well-bg, 7%);
//== Badges
//
//##
@badge-color : #fff;
//** Linked badge text color on hover
@badge-link-hover-color : #fff;
@badge-bg : @gray-light;
//** Badge text color in active nav link
@badge-active-color : @link-color;
//** Badge background color in active nav link
@badge-active-bg : #fff;
@badge-font-weight : bold;
@badge-line-height : 1;
@badge-border-radius : 10px;
//== Breadcrumbs
//
//##
@breadcrumb-padding-vertical : 8px;
@breadcrumb-padding-horizontal : 15px;
//** Breadcrumb background color
@breadcrumb-bg : #f5f5f5;
//** Breadcrumb text color
@breadcrumb-color : #ccc;
//** Text color of current page in the breadcrumb
@breadcrumb-active-color : @gray-light;
//** Textual separator for between breadcrumb elements
@breadcrumb-separator : "/";
//== Carousel
//
//##
@carousel-text-shadow : 0 1px 2px rgba(0, 0, 0, .6);
@carousel-control-color : #fff;
@carousel-control-width : 15%;
@carousel-control-opacity : .5;
@carousel-control-font-size : 20px;
@carousel-indicator-active-bg : #fff;
@carousel-indicator-border-color : #fff;
@carousel-caption-color : #fff;
//== Close
//
//##
@close-font-weight : bold;
@close-color : #000;
@close-text-shadow : 0 1px 0 #fff;
//== Code
//
//##
@code-color : #c7254e;
@code-bg : #f9f2f4;
@kbd-color : #fff;
@kbd-bg : #333;
@pre-bg : #f5f5f5;
@pre-color : @gray-dark;
@pre-border-color : #ccc;
@pre-scrollable-max-height : 340px;
//== Type
//
//##
//** Horizontal offset for forms and lists.
@component-offset-horizontal : 180px;
//** Text muted color
@text-muted : @gray-light;
//** Abbreviations and acronyms border color
@abbr-border-color : @gray-light;
//** Headings small color
@headings-small-color : @gray-light;
//** Blockquote small color
@blockquote-small-color : @gray-light;
//** Blockquote font size
@blockquote-font-size : (@font-size-base * 1.25);
//** Blockquote border color
@blockquote-border-color : @gray-lighter;
//** Page header border color
@page-header-border-color: @gray-lighter;
//** Width of horizontal description list titles
@dl-horizontal-offset : @component-offset-horizontal;
//** Horizontal line color.
@hr-border : @gray-lighter;
// Pingendo variables
@section-spacing : 35px;
// Core variables and mixins
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/mixins.less";
// Reset and dependencies
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/normalize.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/print.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/glyphicons.less";
// Core CSS
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/scaffolding.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/type.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/code.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/grid.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/tables.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/forms.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/buttons.less";
// Components
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/component-animations.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/dropdowns.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/button-groups.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/input-groups.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/navs.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/navbar.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/breadcrumbs.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/pagination.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/pager.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/labels.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/badges.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/jumbotron.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/thumbnails.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/alerts.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/progress-bars.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/media.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/list-group.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/panels.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/responsive-embed.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/wells.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/close.less";
// Components w/ JavaScript
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/modals.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/tooltip.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/popovers.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/carousel.less";
// Utility classes
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/utilities.less";
@import "https://raw.githubusercontent.com/twbs/bootstrap/v3.3.4/less/responsive-utilities.less";
@import "https://raw.githubusercontent.com/Pingendo/pingendo-bootstrap/gh-pages/less/pingendo-custom.less";

<html>
  
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <script type="text/javascript" src="http://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>
    <script type="text/javascript" src="http://netdna.bootstrapcdn.com/bootstrap/3.3.4/js/bootstrap.min.js"></script>
    <link href="http://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.3.0/css/font-awesome.min.css"
    rel="stylesheet" type="text/css">
    <link href="http://pingendo.github.io/pingendo-bootstrap/themes/default/bootstrap.css"
    rel="stylesheet" type="text/css">
  </head>
  
  <body>
    <div class="cover">
      <div class="navbar">
        <div class="container">
          <div class="navbar-header">
            <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#navbar-ex-collapse">
              <span class="sr-only">Toggle navigation</span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
              <span class="icon-bar"></span>
            </button>
            <a class="navbar-brand" href="#"><span>Brand</span></a>
          </div>
          <div class="collapse navbar-collapse" id="navbar-ex-collapse">
            <ul class="nav navbar-nav navbar-right">
              <li class="active">
                <a href="#">Home</a>
              </li>
              <li>
                <a href="#">Contacts</a>
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="background-image-fixed cover-image" style="background-image : url('https://ununsplash.imgix.net/photo-1421284621639-884f4129b61d?w=1024&amp;q=50&amp;fm=jpg&amp;s=9f9c4eb194b84f49e6c6aa624de61ba2')"></div>
      <div class="container">
        <div class="row">
          <div class="col-md-12 text-center">
            <h1 class="text-danger">The Law Office of Sally Suffolk</h1>
            <p class="text-danger">Wills, Estates and Trusts
              <br>
              <br>
              <br>
            </p>
            <br>
            <br>
          </div>
        </div>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <div class="row">
          <div class="col-md-3">
            <img class="img-responsive" src="http://maps.googleapis.com/maps/api/staticmap?center=Tombouctou,Mali&amp;zoom=12&amp;size=200x200&amp;sensor=false">
          </div>
          <div class="col-md-5">
            <p>120 Tremont Street
              <br>Boston, MA 02108
              <br>
              <br>Tel: 251-649-9553
              <br>Email: sally@suffolk,edu</p>
          </div>
          <div class="col-md-4 text-left"></div>
        </div>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <img src="Spring 2016/01 Winter Intersession 2016| Coding the Law/Meg+Ryan+Premiere+Biutiful+Cannes+9lp56fgtzfll.jpg"
            class="img-responsive">
          </div>
          <div class="col-md-6">
            <h1 class="text-primary">Experience</h1>
            <h3>Over 20 Years Experience</h3>
            <p>Divorce is rarely easy, yet it doesn't need to be a traumatic or damaging
              process. Divorce mediation offers a civilized, sensible and affordable
              way to end your marriage while keeping the process short and economical.
              Mediation also lets you and your spouse make your own decisions and control
              the terms of your divorce. As a leading divorce mediation service in Boston
              and throughout Massachusetts, every year we help hundreds of couples to
              file for divorce in a dignified, quick, and affordable way, thus saving
              our clients and their children the emotional and economic burden of ugly
              divorce battles.</p>
          </div>
        </div>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <div class="row">
          <div class="col-md-6">
            <h1 class="text-primary">Training</h1>
            <h3>Schools, Business, and more</h3>
            <p>We train educators and young people in a range of research-based, practical
              programs that build relationships, improve school climate, and increase
              academic success. Programs include: Peer Mediation, Bullying Prevention,
              Student Leadership/Student Mentoring, Restorative Discipline/Restorative
              Practices, Managing Difficult Conversations, Emotional Intelligence, and
              more…</p>
          </div>
          <div class="col-md-6">
            <img src="Spring 2016/01 Winter Intersession 2016| Coding the Law/divorce_mediaion_ma_team.jpg"
            class="img-responsive">
          </div>
        </div>
      </div>
    </div>
    <div class="section">
      <div class="container">
        <div class="row">
          <div class="col-md-12">
            <h1 class="text-center text-primary">Team</h1>
            <p class="text-center">We are a group of skilled individuals.</p>
          </div>
        </div>
        <div class="row">
          <div class="col-md-4">
            <img src="Spring 2016/01 Winter Intersession 2016| Coding the Law/Alan_Jacobs.jpg"
            class="center-block img-circle img-responsive">
            <h3 class="text-center">John James</h3>
            <p class="text-center">Mediator</p>
          </div>
          <div class="col-md-4">
            <img src="Spring 2016/01 Winter Intersession 2016| Coding the Law/Johnson.png"
            class="center-block img-circle img-responsive">
            <h3 class="text-center">Monika Niquax</h3>
            <p class="text-center">Mediator</p>
          </div>
          <div class="col-md-4">
            <img src="Spring 2016/01 Winter Intersession 2016| Coding the Law/Josh.jpg"
            class="center-block img-circle img-responsive">
            <h3 class="text-center">Andrew Sarg</h3>
            <p class="text-center">Mediator</p>
          </div>
        </div>
      </div>
    </div>
  </body>

</html>
/* PINGENDO COMMENT DO NOT REMOVE */

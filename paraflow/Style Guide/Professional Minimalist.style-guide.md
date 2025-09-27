# Surface Light - Charcoal

**Style Overview**: 
- An elegant and minimalist light theme with a simple brand color, #212528.
- This style emphasizes a clean, layered aesthetic by making full use of the **Surface Colors** palette. Instead of traditional dividers or borders, boundaries for nested and adjacent elements are defined by distinct background colors. This technique, combined with modern typography, subtle rounded corners, tight card spacing, and generous internal padding, creates a modern, clean, and distinctive visual hierarchy.

## Colors

- **Primary Colors**: 
  - **color-primary-base**: #212528, for primary buttons, selected states, and accent elements.
  - **color-primary-light**: #4A4D52, for hover states and secondary accents.

- **Background Colors**: 
  - **color-page-background**: #F4F6F8, for the main page background, top, and bottom nav bars.
  - **color-surface-primary**: #FFFFFF, for primary card backgrounds.
  - **color-surface-secondary**: #F4F6F8, for tags on white containers and secondary surface elements.
  - **color-surface-special**: #212528, for important components requiring a dark background.

- **Text Colors**: 
  - **color-text-primary**: #070B11, for main text and most default icon colors.
  - **color-text-secondary**: #888A8B, for secondary text and inactive icons.
  - **color-text-on-dark**: #FFFFFF, for text on dark backgrounds.

- **Functional Colors**: 
  - **color-success**: #3DBF9A, used sparingly for success states, e.g., on success icons only.
  - **color-danger**: #DF6C6C, used sparingly for warning/error states, e.g., on error icons only.

## Typography
- **Font Family**: 
  - **font-family-primary**: `-apple-system, BlinkMacSystemFont, "Segoe UI"`

- **Font Size & Weight**: 
  - **Caption**: 10px / 400
  - **Body**: 12px / 400
  - **Card Title / Emphasized Text**: 14px / 500
  - **Page Title**: 20px / 500
  - **Headline**: 30px / 500
  - **Display**: 40px / 500

- **Line Height**: 1.4

## Border Radius
- **Radius Values & Usage**: 
  - **radius-small (6px)**: For buttons, inputs, tags.
  - **radius-medium (8px)**: For cards, containers, dialogs.
  - **radius-full (50%)**: For avatars, circular buttons.

## Layout & Spacing
- **Principles**:
  - A distinctive layout style is achieved with small gaps(6px) between similar elements (like buttons, cards), generous internal padding(18px).

- **Spacing Scale**: 
  - **Base Unit**: 6px
  - **xs**: 6px - For close arrangement of similar items.
  - **sm**: 12px - For space between icons and text in buttons, space between modules.
  - **md**: 18px - For button and tag padding.
  - **lg**: 24px - For page padding.

## Borders
  - This style uses **no borders**. Element boundaries are distinguished by differences in background color.

## Dividers
  - This style uses **no dividers**. Content areas are separated by background color layers and spacing.

## Shadows & Effects
  - A minimalist approach where element hierarchy is primarily shown through background color layers.
  - Avoid complex shadow effects.

## Assets
### Image
- For normal `<img>`: object-cover
- For `<img>` with:
  - Slight overlay: object-cover brightness-85
  - Heavy overlay: object-cover brightness-50

### Logo
- To protect copyright, do **NOT** use real product logos as a logo for a new product, individual user, or other company products.
- **Icon-based**:
  - **Graphic**: Use a simple, relevant icon from Lucide (e.g., `lucide:calendar` for a scheduler, `lucide:home` for a smart home app).

### Icon
- Use Lucide icons from Iconify.
- To ensure aesthetic layout, each icon should be centered in a square container matching the icon's size. This container is only for layout optimization and does not imply the icon has a background; other properties should be determined based on actual needs.
- Use Tailwind font size to control icon size
- Example:
  ```html
  <div class="flex items-center justify-center bg-transparent w-4 h-4">
  <iconify-icon icon="lucide:flag" class="text-base"></iconify-icon>
  </div>
  ```

## Basic Layout suggestions - Web
<!-- Critical Note: **MUST** follow the layout rules. -->
- Vertical Layout: 
  - body (w-[1440px]) 
    - Header (Fixed height w-full) <!-- bg: color-surface-primary-->
    - Content Container(w-full flex):
      - Left Sider - if present (flex-shrink-0 min-w-fit max-w-xs) <!-- bg: color-surface-secondary-->
      - Main Content Area (flex-1 overflow-x-hidden)
      - Right Sider - if present (flex-shrink-0 min-w-fit max-w-xs) <!-- bg: color-surface-secondary-->
    - Footer - if present (Fixed height w-full)

- Horizontal Layout (at least one of the left/right siders must be present, or both):
  - body (w-[1440px] flex)
    - Left Sider (Optional)<!-- bg: color-surface-primary-->
    - content container:
      - Header (Optional)<!-- bg: color-surface-secondary-->
      - main content area
      - Footer (Optional)
    - Right Sider (Optional)


## Page Layout - Web (*EXTREMELY* important)

```html
<!-- standard implementation for body. A specific body width needs to be defined, which changes based on user requirements -->
<body class="w-[1440px] min-h-[900px] bg-[#F4F6F8] font-[-apple-system,BlinkMacSystemFont,'Segoe UI'] leading-[1.4]">

</body>
```

## Tailwind Component Examples
<!-- Important Note: Use utility classes directly. Do NOT create custom CSS classes or add styles in <style> tags -->
### Basic
- **Progress bars**: h-1.5
- **Button**: <!-- Note: Use flex and items-center for the container-->
  - example 1(text button):
    - button: flex items-center
      - span: Cancel (button copy)
  - example 2(icon button):
    - button: flex items-center
      - icon
- **Lable/Tag/Badge**: 
    - div: flex items-center <!-- Note: Use flex and items-center for the container-->
      - span: All (copy)
- **Segmented button**: 
  - Container: Background color-primary-base, padding p-1
    - Active button: Background color-page-background, text color-text-primary
    - Inactive button: Text color-text-on-dark
### Data Entry

### Container

## Additional Notes

<colors_extraction>
#212528
#4A4D52
#F4F6F8
#FFFFFF
#070B11
#888A8B
#3DBF9A
#DF6C6C
</colors_extraction>
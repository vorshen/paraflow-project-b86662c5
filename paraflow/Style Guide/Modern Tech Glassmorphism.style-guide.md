# Modern Tech Glassmorphism Style Guide

## Colors
### Primary Colors
- **primary-base**: `text-[#2563EB]` or `bg-[#2563EB]` - Cool blue for technical sophistication
- **primary-lighter**: `bg-[#3B82F6]` - Brighter blue for interactive elements
- **primary-darker**: `text-[#1D4ED8]` or `bg-[#1D4ED8]` - Deep blue for emphasis

### Background Colors
- **bg-page**: `bg-gradient-to-br from-[#F8FAFC] via-[#F1F5F9] to-[#E2E8F0]` - Subtle blue-to-gray gradient
- **bg-container-primary**: `bg-white/20 backdrop-blur-md` - Primary glassmorphism containers
- **bg-container-secondary**: `bg-white/10 backdrop-blur-sm` - Secondary glassmorphism surfaces
- **bg-container-inset**: `bg-[#2563EB]/5 backdrop-blur-sm` - Input fields with glass effect
- **bg-container-inset-strong**: `bg-[#2563EB]/10 backdrop-blur-md` - Active states and selections
- **bg-nav**: `bg-white/15 backdrop-blur-xl` - Navigation with enhanced glass effect

### Text Colors
- **color-text-primary**: `text-slate-900/90` - Primary text with strong contrast
- **color-text-secondary**: `text-slate-700/80` - Secondary text information
- **color-text-tertiary**: `text-slate-600/70` - Tertiary supporting text
- **color-text-quaternary**: `text-slate-500/60` - Subtle text elements
- **color-text-on-dark-primary**: `text-white/95` - Text on dark glassmorphism surfaces
- **color-text-on-dark-secondary**: `text-white/80` - Secondary text on dark surfaces
- **color-text-link**: `text-[#06B6D4]` - Cyan accent for links and interactive text

### Functional Colors
- **color-success-default**: `#10B981` - Emerald for success states
- **color-success-light**: `#D1FAE5` - Light emerald background
- **color-error-default**: `#EF4444` - Red for error states
- **color-error-light**: `#FEE2E2` - Light red background
- **color-warning-default**: `#F59E0B` - Amber for warnings
- **color-warning-light**: `#FEF3C7` - Light amber background
- **color-function-default**: `#8B5CF6` - Purple for special functions
- **color-function-light**: `#EDE9FE` - Light purple background

### Accent Colors
- **accent-cyan**: `text-[#06B6D4]` or `bg-[#06B6D4]` - Primary cyan accent
- **accent-cyan-light**: `text-[#67E8F9]` or `bg-[#67E8F9]` - Light cyan for highlights
- **accent-blue-electric**: `text-[#3B82F6]` or `bg-[#3B82F6]` - Electric blue accent
- **accent-purple-tech**: `text-[#8B5CF6]` or `bg-[#8B5CF6]` - Tech purple for categorization

### Data Visualization Charts
- Standard data colors: #E2E8F0, #CBD5E1, #94A3B8, #64748B, #475569, #334155
- Technical accent colors: #06B6D4, #3B82F6, #8B5CF6, #10B981, #F59E0B

## Typography
- **Font Stack**:
  - **font-family-base**: `-apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif` - Modern technical sans-serif
  - **font-family-mono**: `"SF Mono", Monaco, "Cascadia Code", "Roboto Mono", Consolas, "Courier New", monospace` - For code snippets

- **Font Size & Weight**:
  - **Caption**: `text-xs font-normal`
  - **Body small**: `text-sm font-normal`
  - **Body default**: `text-base font-normal`
  - **Card Title / Emphasized Text**: `text-base font-semibold`
  - **Page Title**: `text-2xl font-semibold`
  - **Headline**: `text-4xl font-semibold`
  - **Display**: `text-5xl font-semibold`

- **Line Height**: 1.5

## Border Radius
- **Small**: 8px - Elements inside cards, thumbnails
- **Medium**: 12px - Buttons, inputs, small containers
- **Large**: 16px - Cards, modal containers
- **XL**: 20px - Hero sections, major containers

## Layout & Spacing
- **Spacing Scale**:
- **Base Unit**: 4px
- **Tight**: 8px - Close-related elements
- **Compact**: 12px - List items, component gaps
- **Standard**: 16px - Section spacing, card padding
- **Comfortable**: 24px - Major section separation

## Create Boundaries (contrast of surface color, borders, shadows)
Glassmorphism aesthetic with translucent surfaces, subtle borders, and refined shadow hierarchy

### Borders
- **Glass Border Light**: `border border-white/20` - Subtle glass container borders
- **Glass Border Medium**: `border border-white/30` - Emphasized glass borders
- **Glass Border Strong**: `border border-[#2563EB]/20` - Technical accent borders
- **Active Border**: `border border-[#06B6D4]/40` - Interactive state borders

### Dividers
- **Glass Divider**: `border-t border-white/15` - Subtle glassmorphism dividers
- **Tech Divider**: `border-t border-[#2563EB]/10` - Technical section dividers

### Shadows & Effects
- **Glass Shadow Subtle**: `shadow-[0_8px_32px_rgba(37,99,235,0.08)]` - Subtle glassmorphism depth
- **Glass Shadow Medium**: `shadow-[0_12px_40px_rgba(37,99,235,0.12)]` - Medium glass elevation
- **Glass Shadow Strong**: `shadow-[0_16px_48px_rgba(37,99,235,0.16)]` - Strong glassmorphism presence
- **Tech Glow**: `shadow-[0_0_20px_rgba(6,182,212,0.15)]` - Cyan accent glow effect

## Assets
### Image
- For normal `<img>`: `object-cover`
- For `<img>` with:
  - Slight overlay: `object-cover brightness-95 contrast-105`
  - Heavy overlay: `object-cover brightness-75 contrast-110`

### Logo
- To protect copyright, do **NOT** use real product logos as a logo for a new product, individual user, or other company products.
- **Icon-based**:
  - **Graphic**: Use a simple, tech-relevant FontAwesome Solid icon (e.g., `fa-microchip` for tech blog, `fa-code` for development focus).

### Icon
- Use Lucide icons from Iconify for their modern, technical aesthetic.
- To ensure aesthetic layout, each icon should be centered in a square container matching the icon's size.
- Use Tailwind font size to control icon size
- Example:
  ```html
  <div class="flex items-center justify-center bg-transparent w-5 h-5">
    <iconify-icon icon="lucide:zap" class="text-lg"></iconify-icon>
  </div>
  ```

## Basic Layout - Web
- Vertical Layout: 
  - body (w-[1440px]) 
    - Header (Fixed height w-full) <!-- bg: bg-white/15 backdrop-blur-xl -->
    - Content Container(w-full flex):
      - Left Sider - if present (flex-shrink-0 min-w-fit max-w-xs) <!-- bg: bg-white/10 backdrop-blur-sm -->
      - Main Content Area (flex-1 overflow-x-hidden)
      - Right Sider - if present (flex-shrink-0 min-w-fit max-w-xs) <!-- bg: bg-white/10 backdrop-blur-sm -->
    - Footer - if present (Fixed height w-full)

- Horizontal Layout (at least one of the left/right siders must be present, or both):
  - body (w-[1440px] flex)
    - Left Sider (Optional)<!-- bg: bg-white/15 backdrop-blur-xl -->
    - content container:
      - Header (Optional)<!-- bg: bg-white/10 backdrop-blur-sm -->
      - main content area
      - Footer (Optional)
    - Right Sider (Optional)

## Page Layout - Web
```html
<body class="w-[1440px] min-h-[900px] font-[-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,'Helvetica Neue',Arial,sans-serif] leading-[1.5] bg-gradient-to-br from-[#F8FAFC] via-[#F1F5F9] to-[#E2E8F0]">

</body>
```

## Tailwind Component Examples
### Basic
- **Button**:
  - example 1(glassmorphism text button):
    - button: `flex items-center px-4 py-2 bg-white/20 backdrop-blur-md border border-white/30 rounded-xl hover:bg-white/30 transition-all duration-200`
      - span: Read More (button copy)
  - example 2(glassmorphism icon button):
    - button: `flex items-center justify-center w-10 h-10 bg-white/20 backdrop-blur-md border border-white/30 rounded-xl hover:bg-white/30 transition-all duration-200`
      - icon
- **Label/Tag/Badge**: 
    - div: `flex items-center px-3 py-1 bg-[#06B6D4]/10 backdrop-blur-sm border border-[#06B6D4]/20 rounded-lg`
      - span: Technology (copy)

### Data Entry
- **Progress bars**: `h-2 bg-white/20 backdrop-blur-sm rounded-full overflow-hidden`
- **Checkbox and radio button**
  - default: `bg-white/20 backdrop-blur-sm border border-white/30`
  - checked: `bg-[#2563EB]/20 backdrop-blur-md border border-[#2563EB]/40; text-slate-900/90`

### Container
- **Navigation Menu - horizontal**
    - example 1(Glassmorphism horizontal navigation):
        - Nav Container: `flex items-center gap-8 px-6 py-4 bg-white/15 backdrop-blur-xl border-b border-white/20`
        - Menu Item: `flex items-center gap-2 px-3 py-2 rounded-lg hover:bg-white/20 transition-all duration-200`
          - menu-text: 
          - dropdown-icon (if applicable): `w-4 h-4`
    - example 2(Navigation with glassmorphism sections):
        - Nav Container: `flex items-center justify-between w-full px-6 py-4 bg-white/15 backdrop-blur-xl border-b border-white/20`
        - Left Section: `flex items-center gap-8`
          - Menu Item: `flex items-center gap-2 px-3 py-2 rounded-lg hover:bg-white/20 transition-all duration-200`
        - Right Section: `flex items-center gap-4`
          - Menu Item: `flex items-center gap-2 px-3 py-2 rounded-lg hover:bg-white/20 transition-all duration-200`
          - Notification: `relative flex items-center justify-center w-10 h-10 bg-white/20 backdrop-blur-md border border-white/30 rounded-xl hover:bg-white/30 transition-all duration-200`
            - notification-icon: `w-5 h-5`
            - badge: `absolute -top-1 -right-1 w-5 h-5 bg-[#06B6D4] rounded-full flex items-center justify-center shadow-[0_0_10px_rgba(6,182,212,0.4)]`
              - badge-count: 
          - Avatar: `flex items-center gap-2 p-1 rounded-xl hover:bg-white/20 transition-all duration-200`
            - avatar-image: `w-8 h-8 rounded-full border-2 border-white/30`
            - dropdown-icon: `w-4 h-4`

- **Card**
    - example 1(Glassmorphism vertical card):
        - Card: `bg-white/20 backdrop-blur-md border border-white/30 rounded-2xl p-6 shadow-[0_8px_32px_rgba(37,99,235,0.08)] hover:shadow-[0_12px_40px_rgba(37,99,235,0.12)] transition-all duration-300`
        - Image: `rounded-xl w-full object-cover`
        - Text area: `flex flex-col gap-3 mt-4`
          - card-title: `text-base font-semibold text-slate-900/90`
          - card-subtitle: `text-sm font-normal text-slate-600/70`
    - example 2(Glassmorphism horizontal card):
        - Card: `bg-white/20 backdrop-blur-md border border-white/30 rounded-2xl p-6 flex gap-4 shadow-[0_8px_32px_rgba(37,99,235,0.08)] hover:shadow-[0_12px_40px_rgba(37,99,235,0.12)] transition-all duration-300`
        - Image: `rounded-xl h-full object-cover`
        - Text area: `flex flex-col gap-3 flex-1`
          - card-title: `text-base font-semibold text-slate-900/90`
          - card-subtitle: `text-sm font-normal text-slate-600/70`
    - example 3(Tech blog article card):
        - Card: `flex flex-col gap-4 group cursor-pointer`
        - Image: `rounded-2xl w-full object-cover brightness-95 contrast-105 group-hover:brightness-100 transition-all duration-300`
        - Text area: `flex flex-col gap-3`
          - card-title: `text-base font-semibold text-slate-900/90 group-hover:text-[#2563EB] transition-colors duration-200`
          - card-subtitle: `text-sm font-normal text-slate-600/70`
    - example 4(Featured glassmorphism container):
        - Card: `bg-gradient-to-br from-white/25 to-white/10 backdrop-blur-xl border border-white/30 rounded-2xl p-8 shadow-[0_16px_48px_rgba(37,99,235,0.16)]`

## Additional Notes
This style guide creates a cutting-edge glassmorphism aesthetic perfect for a technology blog, combining transparency effects with technical sophistication. The cool blue primary palette and cyan accents reinforce the tech theme while maintaining professional approachability through medium border radius and refined spacing. The translucent containers with backdrop blur effects create the signature glassmorphism look that feels both modern and innovative.
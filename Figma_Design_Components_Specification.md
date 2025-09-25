# Vision Command Center - Figma Design Components Specification

## 📋 Overview
This document provides comprehensive specifications for recreating the Vision Command Center dashboard components in Figma. All components follow Salesforce Lightning Design System principles.

## 🎨 Design Tokens

### Colors
```css
/* Primary Colors */
--bg-primary: #ffffff
--bg-secondary: #f8f9fa  
--bg-tertiary: #f3f3f3
--text-primary: #181818
--text-secondary: #706e6b
--text-weak: #706e6b

/* Border Colors */
--border-primary: #c9c7c5
--border-secondary: #dddbda

/* Brand Colors */
--slds-c-color-brand: #0176d3
--slds-c-color-success: #04844b
--slds-c-color-warning: #ffb71b
--slds-c-color-error: #c23934

/* Shadow */
--shadow-light: rgba(0,0,0,0.1)
--shadow-medium: rgba(0,0,0,0.15)
```

### Typography
```css
/* Font Family */
Font: 'Salesforce Sans', Arial, sans-serif

/* Font Sizes */
--font-xs: 0.7rem    (11.2px)
--font-sm: 0.8rem    (12.8px)
--font-base: 0.9rem  (14.4px)
--font-md: 1rem      (16px)
--font-lg: 1.1rem    (17.6px)
--font-xl: 1.2rem    (19.2px)
--font-2xl: 1.5rem   (24px)
--font-3xl: 1.8rem   (28.8px)

/* Font Weights */
--font-normal: 400
--font-medium: 500
--font-semibold: 600
--font-bold: 700
```

### Spacing
```css
/* Spacing Scale */
--space-xs: 0.25rem   (4px)
--space-sm: 0.5rem    (8px)
--space-md: 0.75rem   (12px)
--space-lg: 1rem      (16px)
--space-xl: 1.5rem    (24px)
--space-2xl: 2rem     (32px)
--space-3xl: 2.5rem   (40px)
```

### Border Radius
```css
--radius-sm: 4px
--radius-md: 8px
--radius-lg: 12px
--radius-xl: 16px
--radius-2xl: 20px
--radius-full: 50%
```

## 🧩 Core Components

### 1. Header Component
**Specifications:**
- Height: 80px
- Background: Linear gradient (135deg, #0176d3 0%, #4A90E2 100%)
- Padding: 24px 32px
- Color: White
- Contains: Logo, Title, Subtitle

**Elements:**
- **Logo**: 40px height, positioned left
- **Title**: Font size 28.8px, font weight 600
- **Subtitle**: Font size 16px, opacity 0.9

### 2. Navigation Tabs
**Specifications:**
- Height: 48px
- Background: #f8f9fa
- Border bottom: 1px solid #dddbda
- Font size: 14.4px, font weight 500

**Tab States:**
- **Default**: Color #706e6b, padding 12px 24px
- **Active**: Color #0176d3, border-bottom 3px solid #0176d3
- **Hover**: Background rgba(1, 118, 211, 0.05)

### 3. Metric Cards
**Specifications:**
- Width: 280px (minimum)
- Height: 140px
- Background: #ffffff
- Border: 1px solid #dddbda
- Border radius: 12px
- Padding: 24px
- Box shadow: 0 2px 8px rgba(0,0,0,0.08)

**Elements:**
- **Title**: Font size 14.4px, font weight 600, color #181818
- **Value**: Font size 36px, font weight 700
- **Change Indicator**: Font size 12.8px, with trend arrow
- **Mini Chart**: Height 60px, positioned bottom right

**Color Variants:**
- **Positive**: #04844b (green)
- **Negative**: #c23934 (red)  
- **Neutral**: #0176d3 (blue)
- **Warning**: #ffb71b (orange)

### 4. Alert Cards
**Specifications:**
- Width: 100% (flexible)
- Min height: 120px
- Background: #ffffff
- Border: 1px solid #dddbda
- Border radius: 12px
- Padding: 24px
- Border left: 4px solid (severity color)

**Severity Colors:**
- **Critical**: #c23934 (red)
- **High**: #ffb71b (orange)
- **Medium**: #0176d3 (blue)
- **Low**: #04844b (green)

**Elements:**
- **Severity Badge**: Height 24px, padding 4px 12px, border radius 12px
- **Title**: Font size 17.6px, font weight 600
- **Description**: Font size 14.4px, line height 1.5
- **Timestamp**: Font size 12.8px, color #706e6b

### 5. Strategy Board Cards
**Specifications:**
- Width: 320px (minimum)
- Height: 200px
- Background: #ffffff
- Border: 1px solid #dddbda
- Border radius: 16px
- Padding: 24px
- Cursor: pointer
- Transition: all 0.3s ease

**Hover State:**
- Transform: translateY(-4px)
- Box shadow: 0 8px 24px rgba(0,0,0,0.12)

**Elements:**
- **Header**: Contains title and tag
- **Status Indicator**: 8px circle with status color
- **Progress Bar**: Height 6px, border radius 3px
- **Metrics**: 2-column grid
- **Meta Info**: Timeline and owner

**Status Colors:**
- **On Track**: #04844b
- **Needs Attention**: #ffb71b
- **At Risk**: #c23934

### 6. Progress Bars
**Specifications:**
- Height: 6px
- Background: #f3f3f3
- Border radius: 3px
- Fill colors match status

**Progress Text:**
- Font size: 12.8px
- Font weight: 600
- Positioned right

### 7. Status Badges
**Specifications:**
- Height: 24px
- Padding: 4px 12px
- Border radius: 12px
- Font size: 11.2px
- Font weight: 600
- Text transform: uppercase

**Variants:**
- **Success**: Background rgba(4, 132, 75, 0.1), Color #04844b
- **Warning**: Background rgba(255, 183, 27, 0.1), Color #ffb71b
- **Error**: Background rgba(194, 57, 52, 0.1), Color #c23934
- **Info**: Background rgba(1, 118, 211, 0.1), Color #0176d3

### 8. Action Buttons
**Primary Button:**
- Height: 40px
- Padding: 12px 24px
- Background: #0176d3
- Color: white
- Border radius: 8px
- Font weight: 600

**Secondary Button:**
- Height: 40px
- Padding: 12px 24px
- Background: transparent
- Color: #0176d3
- Border: 1px solid #0176d3
- Border radius: 8px

**Button States:**
- **Hover**: Opacity 0.9
- **Active**: Transform scale(0.98)
- **Disabled**: Opacity 0.5

### 9. Charts Container
**Specifications:**
- Background: #ffffff
- Border: 1px solid #dddbda
- Border radius: 12px
- Padding: 24px
- Min height: 300px

**Chart Types:**
- **Line Charts**: 2px stroke width, smooth curves
- **Bar Charts**: 8px border radius on top
- **Doughnut Charts**: 12px thickness
- **Mini Charts**: 60px height, no axes

### 10. Data Tables
**Specifications:**
- Background: #ffffff
- Border: 1px solid #dddbda
- Border radius: 12px

**Table Elements:**
- **Header**: Height 48px, background #f8f9fa, font weight 600
- **Rows**: Height 56px, border bottom 1px solid #f3f3f3
- **Hover**: Background rgba(1, 118, 211, 0.02)

### 11. Input Fields
**Specifications:**
- Height: 40px
- Padding: 12px 16px
- Border: 1px solid #dddbda
- Border radius: 8px
- Font size: 14.4px

**States:**
- **Focus**: Border color #0176d3, outline 3px rgba(1, 118, 211, 0.1)
- **Error**: Border color #c23934
- **Disabled**: Background #f3f3f3, opacity 0.6

### 12. Modal/Dialog
**Specifications:**
- Width: 600px (default)
- Background: #ffffff
- Border radius: 16px
- Box shadow: 0 16px 48px rgba(0,0,0,0.2)
- Backdrop: rgba(0,0,0,0.5)

**Elements:**
- **Header**: Height 64px, padding 24px, border bottom 1px solid #f3f3f3
- **Body**: Padding 24px
- **Footer**: Height 80px, padding 24px, border top 1px solid #f3f3f3

### 13. Agentforce Chat Panel
**Specifications:**
- Width: 400px
- Height: 100vh
- Background: #f8f9fa
- Border left: 1px solid #dddbda

**Elements:**
- **Header**: Height 64px, background #0176d3, color white
- **Messages**: Flex 1, padding 16px, overflow auto
- **Input**: Height 80px, padding 16px

**Message Bubbles:**
- **User**: Background #0176d3, color white, margin left auto
- **Agent**: Background #ffffff, border 1px solid #dddbda
- Max width: 85%, border radius 12px, padding 12px

### 14. Loading States
**Spinner:**
- Size: 24px
- Color: #0176d3
- Animation: 1s linear infinite

**Skeleton:**
- Background: #f3f3f3
- Border radius: 4px
- Animation: pulse 1.5s ease-in-out infinite

## 📱 Responsive Breakpoints

```css
/* Breakpoints */
--mobile: 768px
--tablet: 1024px
--desktop: 1200px
--large: 1440px

/* Grid System */
--container-max-width: 1200px
--grid-columns: 12
--grid-gap: 24px
```

## 🎯 Component Variants

### Metric Card Variants
1. **Revenue Metric** - Large value, currency format, trend indicator
2. **Percentage Metric** - Progress bar, percentage value
3. **Count Metric** - Integer value, comparison indicator
4. **Status Metric** - Color-coded status, description text

### Alert Card Variants
1. **System Alert** - Technical issues, error codes
2. **Business Alert** - KPI deviations, trend warnings  
3. **Customer Alert** - Support issues, satisfaction drops
4. **Operational Alert** - Process failures, capacity issues

### Strategy Board Variants
1. **Growth Strategy** - Revenue focus, green theme
2. **Crisis Recovery** - Urgent priority, red theme
3. **Customer Experience** - CX metrics, orange theme
4. **Revenue Protection** - Financial focus, blue theme

## 🔧 Interactive States

### Hover Effects
- **Cards**: translateY(-4px), enhanced shadow
- **Buttons**: opacity 0.9, subtle scale
- **Links**: color change, underline

### Loading States
- **Shimmer**: Linear gradient animation
- **Spinner**: Rotating animation
- **Skeleton**: Pulse animation

### Focus States
- **Interactive Elements**: 3px outline, brand color
- **Form Fields**: Border highlight, shadow

## 📊 Chart Specifications

### Color Palette for Charts
```css
/* Chart Colors */
--chart-primary: #0176d3
--chart-success: #04844b  
--chart-warning: #ffb71b
--chart-error: #c23934
--chart-info: #6366f1
--chart-purple: #8b5cf6
--chart-pink: #ec4899
--chart-teal: #14b8a6
```

### Chart Dimensions
- **Dashboard Charts**: 400px × 300px
- **Mini Charts**: 100px × 60px
- **Full Width Charts**: 100% × 400px

## 🎨 Figma Setup Instructions

### 1. Create Design System
1. Set up color styles using the color tokens above
2. Create text styles for all typography variants
3. Set up effect styles for shadows and glows
4. Create grid styles with 24px gutters

### 2. Component Library Structure
```
📁 Components
  📁 Layout
    - Header
    - Navigation
    - Sidebar
    - Footer
  📁 Cards
    - Metric Card
    - Alert Card  
    - Strategy Board Card
  📁 Forms
    - Input Field
    - Button (Primary/Secondary)
    - Dropdown
    - Checkbox
  📁 Data Display
    - Progress Bar
    - Status Badge
    - Data Table
    - Chart Container
  📁 Feedback
    - Loading Spinner
    - Skeleton Loader
    - Toast Notification
  📁 Navigation
    - Tab Navigation
    - Breadcrumb
    - Pagination
  📁 Overlays
    - Modal
    - Tooltip
    - Popover
```

### 3. Auto Layout Setup
- Use Auto Layout for all components
- Set proper spacing between elements
- Configure resizing behavior (Fill/Hug/Fixed)

### 4. Component Properties
Create variants for:
- **States**: Default, Hover, Active, Disabled
- **Sizes**: Small, Medium, Large
- **Types**: Primary, Secondary, Success, Warning, Error
- **Content**: Text variations, icon presence

### 5. Responsive Design
- Create responsive variants for mobile/tablet/desktop
- Use constraints and auto layout for flexible designs
- Test components at different screen sizes

## 📋 Component Checklist

### Essential Components to Create:
- [ ] Header with logo and navigation
- [ ] Tab navigation system
- [ ] Metric cards (4 variants)
- [ ] Alert cards (4 severity levels)
- [ ] Strategy board cards
- [ ] Progress bars and status badges
- [ ] Action buttons (primary/secondary)
- [ ] Chart containers
- [ ] Data tables
- [ ] Input fields and forms
- [ ] Agentforce chat panel
- [ ] Modal dialogs
- [ ] Loading states

### Advanced Components:
- [ ] Interactive dashboards layouts
- [ ] Chart components with data visualization
- [ ] Complex form layouts
- [ ] Multi-step workflows
- [ ] Responsive grid systems

This specification provides everything needed to recreate the Vision Command Center dashboard in Figma with pixel-perfect accuracy and full design system consistency.

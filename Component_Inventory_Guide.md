# Vision Command Center - Component Inventory Guide

## 📸 Visual Component Reference

This guide provides a comprehensive inventory of all UI components used in the Vision Command Center dashboards, organized by category with exact specifications for Figma recreation.

## 🏗️ Layout Components

### 1. Main Header
**Location**: Top of every dashboard page
**Dimensions**: Full width × 80px height
**Key Elements**:
- Salesforce logo (40px height)
- Main title "Vision Command Center" (28.8px, weight 600)
- Subtitle "Future of Business Intelligence" (16px, opacity 0.9)
- Gradient background: #0176d3 → #4A90E2

### 2. Tab Navigation
**Location**: Below header
**Dimensions**: Full width × 48px height
**Tabs**: Glance | Monitor | Analyze | Act
**States**: Default (gray), Active (blue with bottom border), Hover

### 3. Content Grid System
**Layout**: CSS Grid with 24px gaps
**Responsive**: 1-4 columns based on screen size
**Container**: Max-width 1200px, centered

## 📊 Data Display Components

### 4. Metric Cards (Primary KPIs)
**Dimensions**: 280px × 140px minimum
**Found in**: Glance tab, top row
**Variants**:
- Revenue metrics (currency format)
- Percentage metrics (with progress bars)
- Count metrics (integers with change indicators)
- Status metrics (color-coded)

**Example Metrics**:
- Total Revenue: $78M (green, +12.3%)
- Customer Satisfaction: 3.2/5 (red, -28.1%)
- Active Customers: 15,247 (blue, +5.2%)
- Support Tickets: 2,847 (orange, +31.7%)

### 5. Mini Charts (Inside Metric Cards)
**Dimensions**: 100px × 60px
**Types**: Line charts, bar charts, trend indicators
**Colors**: Match parent metric card status color
**Position**: Bottom right of metric card

### 6. Alert Cards (Critical Issues)
**Dimensions**: Full width × variable height (min 120px)
**Location**: Monitor tab
**Severity Levels**:
- **Critical**: Red left border (#c23934)
- **High**: Orange left border (#ffb71b)
- **Medium**: Blue left border (#0176d3)
- **Low**: Green left border (#04844b)

**Content Structure**:
- Severity badge (top left)
- Alert title (17.6px, weight 600)
- Description (14.4px, line-height 1.5)
- Timestamp (12.8px, gray)
- Action buttons (if applicable)

### 7. Strategy Board Cards
**Dimensions**: 320px × 200px minimum
**Location**: Act tab
**Interactive**: Hover effects, clickable
**Content**:
- Header with title and category tag
- Status indicator (colored dot)
- Progress bar with percentage
- Key metrics (2-column grid)
- Meta info (timeline, owner)

**Status Colors**:
- On Track: Green (#04844b)
- Needs Attention: Orange (#ffb71b)
- At Risk: Red (#c23934)

### 8. Data Tables
**Location**: Various tabs for detailed data
**Structure**:
- Header row (48px height, gray background)
- Data rows (56px height)
- Hover states (light blue background)
- Sortable columns
- Pagination controls

## 🎛️ Interactive Components

### 9. Primary Buttons
**Dimensions**: 40px height × variable width
**Padding**: 12px horizontal, 12px vertical
**Colors**: Blue background (#0176d3), white text
**States**: Default, Hover (opacity 0.9), Active, Disabled

### 10. Secondary Buttons
**Dimensions**: Same as primary
**Style**: Transparent background, blue border and text
**Usage**: Cancel actions, secondary CTAs

### 11. Status Badges
**Dimensions**: 24px height × auto width
**Padding**: 4px horizontal, 8px vertical
**Border Radius**: 12px (pill shape)
**Font**: 11.2px, weight 600, uppercase
**Colors**: Match semantic color system

### 12. Progress Bars
**Dimensions**: Variable width × 6px height
**Background**: Light gray (#f3f3f3)
**Fill**: Status-dependent color
**Border Radius**: 3px
**Usage**: Progress tracking, completion rates

### 13. Input Fields
**Dimensions**: Variable width × 40px height
**Padding**: 12px horizontal
**Border**: 1px solid gray, 8px border radius
**States**: Default, Focus (blue border), Error (red border)

## 🗨️ Communication Components

### 14. Agentforce Chat Panel
**Dimensions**: 400px width × full height
**Position**: Right side of strategy board detail pages
**Structure**:
- Header (64px, blue background)
- Messages area (flex grow, scrollable)
- Input field (80px height)

**Message Bubbles**:
- User: Blue background, right-aligned
- Agent: White background, left-aligned
- Max width: 85% of container
- Border radius: 12px, padding: 12px

### 15. Notification Toasts
**Position**: Top right corner
**Dimensions**: 400px width × auto height
**Types**: Success (green), Warning (orange), Error (red), Info (blue)
**Auto-dismiss**: 5 seconds

## 📱 Responsive Components

### 16. Mobile Navigation
**Breakpoint**: < 768px
**Style**: Hamburger menu, collapsible sidebar
**Touch targets**: Minimum 44px height

### 17. Responsive Cards
**Behavior**: Stack vertically on mobile, grid on desktop
**Minimum width**: 280px
**Maximum width**: 400px per card

### 18. Flexible Data Tables
**Mobile**: Horizontal scroll or card layout
**Tablet**: Reduced columns
**Desktop**: Full table view

## 🎨 Visual Effects & States

### 19. Loading States
**Spinner**: 24px, blue color, rotating animation
**Skeleton**: Gray placeholder blocks with pulse animation
**Progress**: Linear progress bar for longer operations

### 20. Hover Effects
**Cards**: Slight elevation (4px up), enhanced shadow
**Buttons**: Opacity change or subtle scale
**Interactive elements**: Color transitions

### 21. Focus States
**Keyboard navigation**: 3px blue outline
**Form fields**: Blue border highlight
**Buttons**: High contrast outline

## 📐 Spacing & Layout Rules

### Grid System
- **Container**: 1200px max-width, centered
- **Columns**: 12-column grid system
- **Gaps**: 24px between components
- **Margins**: 32px page margins on desktop, 16px on mobile

### Vertical Rhythm
- **Section spacing**: 40px between major sections
- **Component spacing**: 24px between related components
- **Element spacing**: 16px between related elements
- **Text spacing**: 8px between text elements

## 🎯 Component Priority for Figma

### Phase 1 (Essential)
1. ✅ Header component
2. ✅ Tab navigation
3. ✅ Metric cards (4 variants)
4. ✅ Primary/secondary buttons
5. ✅ Status badges
6. ✅ Progress bars

### Phase 2 (Core Features)
1. ✅ Alert cards (4 severity levels)
2. ✅ Strategy board cards
3. ✅ Data tables
4. ✅ Input fields
5. ✅ Loading states

### Phase 3 (Advanced)
1. ✅ Agentforce chat panel
2. ✅ Modal dialogs
3. ✅ Chart containers
4. ✅ Responsive variants
5. ✅ Interactive states

## 📋 Figma File Organization

### Recommended Structure:
```
📁 Vision Command Center Design System
  📁 🎨 Design Tokens
    - Colors
    - Typography
    - Spacing
    - Shadows
  📁 🧩 Components
    📁 Layout
    📁 Navigation  
    📁 Data Display
    📁 Forms & Inputs
    📁 Feedback
    📁 Charts
  📁 📱 Templates
    📁 Dashboard Layouts
    📁 Detail Pages
    📁 Mobile Views
  📁 🎭 Examples
    📁 CXO Dashboard
    📁 Service VP Dashboard
    📁 Strategy Boards
```

## 🔗 Implementation Notes

### Auto Layout Usage
- All components should use Auto Layout for flexibility
- Set proper spacing and padding tokens
- Configure resizing behavior (Fill/Hug/Fixed)

### Component Properties
Create variants for:
- **States**: Default, Hover, Active, Disabled, Loading
- **Sizes**: Small, Medium, Large (where applicable)
- **Types**: Primary, Secondary, Success, Warning, Error
- **Content**: Different text lengths, with/without icons

### Accessibility Considerations
- Minimum 44px touch targets for mobile
- 4.5:1 color contrast ratio for text
- Clear focus indicators
- Semantic structure for screen readers

This comprehensive component inventory provides everything needed to recreate the Vision Command Center dashboards in Figma with complete design system consistency.

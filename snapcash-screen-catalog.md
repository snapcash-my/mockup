# SnapCash Application Screen Inventory & Visual Catalog

This document provides a highly detailed, page-by-page visual, textual, and functional inventory of the **31 selected screenshots** from the SnapCash application. It catalogs key text strings, input fields, interactive states, color-coded status indicators, and operational logic visible in each interface.

---

## Part 1: Onboarding & Authentication Flow

### 1. Onboarding Screen (Splash State 1)
*   **Source File:** `Screenshot 2026-05-07 at 5.07.41 PM.png`
*   **Viewport Type:** Mobile Portrait (Clean)
*   **Visual Assets:**
    *   Centrally-aligned circular icon featuring an orange/salmon map icon.
    *   Dot indicator below the text showing page 1 of onboarding (first dot active orange, subsequent two dots light grey).
*   **On-Screen Text:**
    *   **Heading:** "Find Nearby Merchants."
    *   **Description:** "Explore a map of trusted local stores offering cash withdrawal services."
    *   **Text Links:** "I already have an account" (orange text link at the very bottom).
*   **Interactive Controls:**
    *   Orange "Continue" button.
    *   Orange "Get Started" button.
    *   "I already have an account" click trigger.

### 2. Onboarding Screen (Splash State 1 - Desktop Frame)
*   **Source File:** `Screenshot 2026-05-07 at 5.07.58 PM.png`
*   **Viewport Type:** Desktop/Tablet wrapped inside a light grey border frame.
*   **Visual Assets & Text:** Identical to the mobile onboarding screen (map icon, heading, description, and dots).
*   **Functional Role:** Demonstrates cross-platform viewport scaling for wider screens.

### 3. Login Screen (Empty State)
*   **Source File:** `Screenshot 2026-05-07 at 5.08.08 PM.png`
*   **Visual Assets:**
    *   Orange SnapCash brand logo (a conversation bubble showing a white dollar sign `$`).
    *   "Log in to SnapCash" sub-header.
*   **On-Screen Text:**
    *   "Sign in with Google" (orange background button with white Google logo).
    *   "Sign in with Apple" (black background button with white Apple logo).
    *   Divider text: "Or continue with email"
    *   Labels: "Email", "Password", "Forgot password?" (orange utility link).
*   **Interactive Controls & Inputs:**
    *   Email text input field with placeholder `you@example.com`.
    *   Password text input field with placeholder `••••••••`.
    *   "Sign in with Email" button, currently in an inactive, semi-transparent light salmon color (blocked until text is entered).

### 4. Login Screen (Filled State)
*   **Source File:** `Screenshot 2026-05-07 at 5.08.24 PM.png`
*   **Visual Assets:** Same logo and layout as the empty state.
*   **Interactive Controls & Inputs:**
    *   Email input field now populated with: `fadlisaad@gmail.com`.
    *   Password field now filled with masked characters (`••••••••`).
    *   "Sign in with Email" button is now fully active (solid dark orange color), allowing submission.

### 5. Login Verification Interface
*   **Source File:** `Screenshot 2026-05-07 at 5.08.39 PM.png`
*   **Visual Assets & Layout:** Secondary authentication status interface verifying email/password matching.
*   **Functional Role:** Internal routing screen during the authorization and session generation process.

---

## Part 2: Customer Discovery & Request Cash Flow

### 6. Available Merchants (List View - Stores Tab)
*   **Source File:** `Screenshot 2026-05-07 at 5.08.49 PM.png`
*   **Application Version Indicator:** `v1.0.12` centered above the bottom navigation bar.
*   **Visual Assets:**
    *   Top Bar: Title "Available Merchants" with a "Map View" toggle button (top right).
    *   Segmented Control: "Stores" tab active (white background with shadow), "Mobile Merchants" tab inactive (grey background).
    *   Store Radius Slider: Currently configured at "Store Radius: 10 km". 
    *   Sub-label: "Adjust the radius to find static stores further away."
*   **Merchant Card Details ("Kedai Runcit Mawar"):**
    *   Location pin icon with text: "Jalan Sultan Ismail, Kuala Lumpur".
    *   Clock icon: "8:00 AM - 9:00 PM".
    *   Star icon: "3.9 (45 ratings)".
    *   Walking/Compass icon: "8.8 km (106 min)".
    *   Orange button: "View Details".
*   **Bottom Navigation Bar:**
    *   "Explore" tab highlighted in orange with a magnifying glass icon.
    *   "History" tab inactive (clock icon).
    *   "Profile" tab inactive (user silhouette icon).

### 7. Available Merchants (List View - Mobile Merchants Tab)
*   **Source File:** `Screenshot 2026-05-07 at 5.09.03 PM.png`
*   **Segmented Control:** "Mobile Merchants" tab is now active; "Stores" tab is inactive.
*   **Merchant Card Details ("Agile Technoprenuer Sdn Bhd"):**
    *   Label: "Mobile Merchant".
    *   Clock icon: "9 AM - 5 PM Daily".
    *   Star icon: "4.5 (6 ratings)".
    *   Orange button: "View Details".
*   **Navigation & Version:** Identical Bottom Navigation with "Explore" active; App version `v1.0.12`.

### 8. Merchant Detail View (Request Form Inactive)
*   **Source File:** `Screenshot 2026-05-07 at 5.09.24 PM.png`
*   **Merchant Header Block ("Agile Technoprenuer Sdn Bhd"):**
    *   Green "Open" status badge.
    *   "Mobile Merchant" subtitle.
    *   Phone icon and phone number: `+60321432143`.
    *   Clock icon: "Operating Hours: 9 AM - 5 PM Daily".
    *   Star icon: "Rating: 4.5 (6 reviews)".
*   **Request Cash Input Section:**
    *   Subtitle: "Enter the amount you wish to withdraw".
    *   Text input field labeled "Amount (RM)" displaying a default state of `RM 0.00`.
    *   Limits subtitle: "Min: RM 10.00 | Max: RM 1000.00".
    *   Quick Select buttons: `RM 10`, `RM 20`, `RM 30`, `RM 50`, `RM 100`, `RM 200`, and `RM 500`.
    *   Submit Button: "Request Cash" in a disabled, semi-transparent light salmon state.
    *   Disclaimer: "By requesting cash, you agree to pay the merchant the total amount via DuitNow QR."
*   **Secondary Buttons:** "Back to Merchants" text button with left arrow icon.

### 9. Merchant Detail View (Request Form Active)
*   **Source File:** `Screenshot 2026-05-07 at 5.09.49 PM.png`
*   **Interactive State Changes:**
    *   Quick Select button `RM 200` has been tapped, changing to a solid orange background.
    *   "Amount (RM)" text input field automatically updates to `RM 200`.
*   **Dynamic Cost Calculations Card:**
    *   "Withdrawal Amount: RM 200.00"
    *   "Service Fee: RM 1.00"
    *   "Total to Pay: RM 201.00"
*   **Submit Button:** "Request Cash" transitions to an active, solid orange state.

### 10. Customer Waiting Screen (Full Screen Progress)
*   **Source File:** `Screenshot 2026-05-07 at 5.09.58 PM.png`
*   **Visual Assets:**
    *   Centered orange-accented circular progress indicator with an analog clock icon inside.
    *   Header: "Waiting for Merchant"
    *   Sub-header: "Your cash request is being processed"
    *   Merchant Context: "Agile Technoprenuer Sdn Bhd is reviewing your request"
*   **Countdown Bar:**
    *   Solid orange progress track with "Request expires in: 4:42" overlay text.
*   **Summary Box:**
    *   Withdrawal Amount: RM 200.00
    *   Service Fee: RM 1.00
    *   Total to Pay: RM 201.00
*   **System Advice Card:**
    *   "The merchant will either accept or decline your request shortly. You can cancel your request at any time."
*   **Utility Button:** "Cancel Request" bordered button.

### 11. Customer Waiting Screen (With Bottom Navigation)
*   **Source File:** `Screenshot 2026-05-07 at 5.11.27 PM.png`
*   **Interactive Changes:**
    *   Countdown timer is at "4:32".
    *   Bottom navigation bar is now overlaid, showing "History" (with the clock icon) highlighted.
*   **Purpose:** Allows customers to navigate away to look at previous transactions while their current transaction is pending.

---

## Part 3: Merchant Dashboard & Request Management Flow

### 12. Merchant Dashboard (Pending Request Notification)
*   **Source File:** `Screenshot 2026-05-07 at 5.11.50 PM.png`
*   **Merchant Status Control:**
    *   Title "Merchant Dashboard".
    *   "Store Status: Online" block with a toggled-on (orange) switch.
    *   Description: "Toggle to set your store as offline for cash withdrawals."
*   **Sub-Navigation Tabs:**
    *   "Transactions" tab active (white background with shadow).
    *   "Ratings" tab inactive (grey background).
*   **Transaction Queue:**
    *   Section Header: "Latest Transaction Requests (Review recent cash withdrawal requests from customers)."
    *   **Row 1 (Active Request):**
        *   Customer Name: "Fadli Saad"
        *   Date: "May 7, 2026 at 5:09 PM"
        *   Ref ID: `Ref: SC-260507090927-81b835`
        *   Value: `RM 200.00`
        *   Status Badge: "Pending" (yellow background, dark text).
    *   **Rows 2-5 (Completed / Past Requests):**
        *   Row 2: "Fadli Saad", "May 6, 2026 at 11:53 AM", `RM 200.00`, Status: "Completed" (green badge).
        *   Row 3: "Fadli Saad", "May 5, 2026 at 10:07 AM", `RM 30.00`, Status: "Completed" (green badge).
        *   Row 4: "Fadli Saad", "May 4, 2026 at 5:39 PM", `RM 20.00`, Status: "Cancelled" (red badge).
        *   Row 5: "Fadli Saad", "May 4, 2026 at 5:16 PM", `RM 20.00`, Status: "Cancelled" (red badge).
*   **Bottom Navigation Bar (Merchant Side):**
    *   "Merchant" tab highlighted (orange home icon).
    *   "Profile" tab inactive (user silhouette icon).

### 13. Merchant Review Request Interface
*   **Source File:** `Screenshot 2026-05-07 at 5.12.06 PM.png`
*   **Visual Assets:**
    *   Top Bar: "Back to Dashboard" text button with left arrow icon.
    *   Gold hourglass icon centered at the top.
    *   Title: "Transaction Request"
    *   Date: "May 7, 2026 at 5:09 PM"
    *   Status Badge: "Pending" (yellow background).
*   **Request Metadata Table:**
    *   Merchant Ref: `SC-260507090927-81b835`
    *   Customer: "Fadli Saad"
    *   Withdrawal Amount: "RM 200.00"
    *   Service Fee: "RM 1.00"
    *   **Total Customer Pays:** "RM 201.00" (rendered in large bold typeface).
*   **Interactive Controls:**
    *   Green Button: "Approve Request" (solid).
    *   White Button with Red Outline: "Reject Request".
    *   Help Text: "Manage this transaction request. Approving will notify the customer to proceed to your location."

### 14. Merchant Dashboard (Request Approved State)
*   **Source File:** `Screenshot 2026-05-07 at 5.12.14 PM.png`
*   **Visual Updates:**
    *   Under "Latest Transaction Requests," Row 1 (Fadli Saad, May 7, 2026, RM 200.00) now displays a blue status badge labeled "Accepted".
    *   All other past transactions (Completed, Cancelled) remain listed below.

---

## Part 4: Real-Time Payment & Handover Flow

### 15. Customer Map Routing & Directions Interface
*   **Source File:** `Screenshot 2026-05-07 at 5.12.33 PM.png`
*   **Approval Confirmation Block:**
    *   Green checkmark circle.
    *   Heading: "Request Accepted!"
    *   Description: "Your cash request has been approved by the merchant"
*   **Urgency & Routing Indicators:**
    *   Green instruction banner: "Please proceed to the merchant within 15 minutes".
    *   Red timer warning block: "Time to reach merchant: 12:34" (clock icon overlay).
*   **Merchant Identity & Contact:**
    *   Merchant: "Agile Technoprenuer Sdn Bhd"
    *   Badge: "Mobile Merchant"
    *   Phone Button: `+60321432143` (phone icon).
*   **Embedded Navigation Map:**
    *   Interactive map showing current layout around Damansara Utama (The Starling area).
    *   Red location drop pin representing the merchant.
    *   Floating Distance Badge: "Distance 92m" with an orange directional arrow.
    *   Buttons below Map: "Directions" (grey outline) and "Payment" (white card outline).
*   **Summary Footer:** Shows RM 200.00 withdrawal, RM 1.00 fee, RM 201.00 total.

### 16. Payment Method Selection (Default Location Locked)
*   **Source File:** `Screenshot 2026-05-07 at 5.12.55 PM.png`
*   **Visual Focus:** Scrolled to the bottom half of the map interface.
*   **Select Payment Method Options:**
    *   **Option 1:** "QR Code Payment" (radio unchecked). Description: "Scan QR code with any banking app". Shows a orange/red QR code icon.
    *   **Option 2:** "FPX Online Banking" (radio unchecked). Description: "Pay directly from your bank account". Shows an orange bank building icon.
*   **Payment Action Button:**
    *   Disabled, light salmon color button: "Move to merchant location to pay".
    *   Under-text warning: "You must be at the merchant's location to initiate payment".

### 17. FPX Bank List Expanded
*   **Source File:** `Screenshot 2026-05-07 at 5.13.36 PM.png`
*   **Interactive Changes:**
    *   "FPX Online Banking" is selected (orange radio checked).
    *   An expanded vertical dropdown lists available bank institutions:
        *   `AGRONet`
        *   `Alliance Bank (Personal)`
        *   `AmBank`
        *   `Bank Islam`
        *   `Bank Muamalat`
        *   `Bank of China`
    *   Button remain locked: "Move to merchant location to pay" remains inactive.

### 18. Merchant-Side Transition (Awaiting Customer Arrival)
*   **Source File:** `Screenshot 2026-05-07 at 5.14.29 PM.png`
*   **Header Block:** Same transaction detail block with "Accepted" blue badge (May 7, 2026).
*   **Customer Proximity Prompts:**
    *   Blue alert card: "Customer is on their way. Prepare RM 200.00 cash."
    *   Dynamic QR Container: "Show this DuitNow QR to the customer" with an active loading wheel icon.
*   **Controls:** "Cancel Transaction" (red outline button).

### 19. Customer Proximity Lock Released (Arrived State)
*   **Source File:** `Screenshot 2026-05-07 at 5.15.39 PM.png`
*   **Customer Interface Update:**
    *   The map distance is now "Distance 17m".
    *   Blue alert badge displays: "You are at the merchant's location!" (unlocking the proximity sensor).
    *   Under bank selection, bank option `SBI Bank A` is now chosen (marked with an orange bar and checked tick).
*   **Payment Action Button:**
    *   The disabled "Move to merchant" button transforms into an active, bright orange button labeled "Make Payment".

### 20. Merchant-Side Handover Ready Screen
*   **Source File:** `Screenshot 2026-05-07 at 5.15.21 PM.png`
*   *Note: Represents the terminal state preparing the transaction completion on the merchant backend.*

### 21. Customer Payment Successful Confirmation
*   **Source File:** `Screenshot 2026-05-07 at 5.16.12 PM.png`
*   **Visual Assets:** Large green checkmark icon.
*   **On-Screen Text:**
    *   Header: "Payment Successful!"
    *   Subtitle: "Your FPX payment was approved. The merchant has been notified — please proceed to collect your cash."
*   **Receipt Details:**
    *   Merchant: "Agile Technoprenuer Sdn Bhd"
    *   Withdrawal Amount: "RM 200.00"
    *   Total Paid: "RM 201.00"
    *   Date: "May 7, 2026 at 5:09 PM"
*   **Call-to-Action Buttons:**
    *   Orange Button: "Rate This Transaction"
    *   White Outline Button: "View Transaction History"
    *   App version `v1.0.12` centered at the bottom.

### 22. Merchant-Side Completed Transaction State
*   **Source File:** `Screenshot 2026-05-07 at 5.16.24 PM.png`
*   **Visual Assets:** Green checkmark icon.
*   **On-Screen Text:**
    *   Title: "Transaction Request"
    *   Status Badge: "Completed" (green background).
    *   Green card: "This transaction has been completed"
*   **Summary:** Shows identical totals (RM 200.00, Fee RM 1.00, Total RM 201.00).

### 23. Customer Experience Rating Screen
*   **Source File:** `Screenshot 2026-05-07 at 5.16.39 PM.png`
*   **Visual Assets:**
    *   Title: "Rate Your Experience"
    *   Question: "How was your experience with Agile Technoprenuer Sdn Bhd?"
    *   Five large yellow star graphics (all 5 lit up).
    *   Text feedback indicator: "Excellent (You rated this 5 stars)".
*   **Feedback Inputs:**
    *   Text input field with heading "Additional Comments (Optional)" populated with text: `Great`.
*   **Submit Controls:**
    *   Solid orange button "Submit Rating".
    *   Footer: "Your feedback helps improve the SnapCash community. v1.0.12"

---

## Part 5: User Profile & Account Settings Flow

### 24. Transaction History (Consolidated Log)
*   **Source File:** `Screenshot 2026-05-07 at 5.16.55 PM.png`
*   **Visual Layout:**
    *   Header: "Transaction History" with a dropdown filter button set to "All Statuses".
    *   List view of all historical customer records.
*   **Transactions Detailed:**
    *   Row 1: Agile Technoprenuer Sdn Bhd | May 7, 2026 at 5:09 PM | `-RM 200.00` | "Completed" (green badge) | Ref SC-260507090927-81b835
    *   Row 2: Agile Technoprenuer Sdn Bhd | May 6, 2026 at 11:53 AM | `-RM 200.00` | "Completed" (green badge)
    *   Row 3: Agile Technoprenuer Sdn Bhd | May 5, 2026 at 10:07 AM | `-RM 30.00` | "Completed" (green badge)
    *   Row 4: Agile Technoprenuer Sdn Bhd | May 4, 2026 at 5:39 PM | `-RM 20.00` | "Cancelled" (red badge)
    *   Row 5: Agile Technoprenuer Sdn Bhd | May 4, 2026 at 5:16 PM | `-RM 20.00` | "Cancelled" (red badge)
*   **Bottom Navigation Bar:** "History" tab active (orange clock icon).

### 25. Historic Receipt Details View
*   **Source File:** `Screenshot 2026-05-07 at 5.17.06 PM.png`
*   **Visual Assets:**
    *   Top Bar: "Back to History" with left arrow.
    *   Large green checkmark badge.
    *   Header: "Agile Technoprenuer Sdn Bhd" | "May 7, 2026 at 5:09 PM"
    *   Status Badge: "Completed" (green).
*   **Record Table:**
    *   Merchant Ref: `SC-260507090927-81b835`
    *   Withdrawal Amount: "RM 200.00"
    *   Service Fee: "RM 1.00"
    *   **Total Paid:** "RM 201.00" (bolded)
*   **Stored User Rating Card:**
    *   5 out of 5 stars displayed.
    *   Quote box displaying the text: `“Great”`.

### 26. Profile Home Dashboard
*   **Source File:** `Screenshot 2026-05-07 at 5.17.17 PM.png`
*   **User Identity Block:**
    *   Circular avatar photo containing a real-world portrait of a man and a child.
    *   Display Name: "Fadli Saad"
    *   User Email: `fadlisaad@gmail.com`
*   **Connected Accounts Card:**
    *   Heading "Connected Accounts".
    *   Green checkmarks indicating: "Email" connected, "Google" connected.
*   **List Options Menu (with Right Chevrons):**
    *   "Account Information"
    *   "Apply to be a Merchant"
    *   "Security"
    *   "Notifications"
    *   "Help & Support"
*   **Critical Utility Buttons:**
    *   Red solid button: "Log Out" (white exit icon).
    *   White button with red outline: "Delete Account" (red trash can icon).
*   **Bottom Navigation Bar:** "Profile" tab active (orange profile icon).

### 27. Account Information Form
*   **Source File:** `Screenshot 2026-05-07 at 5.17.27 PM.png`
*   **On-Screen Fields:**
    *   Avatar URL field: placeholder `https://example.com/avatar.jpg`.
    *   First Name: text field containing `Fadli`.
    *   Last Name: text field containing `Saad`.
    *   Email: greyed-out uneditable text field showing `fadlisaad@gmail.com` with helper caption "Email cannot be changed here."
    *   Phone Number: text field containing `60126471057` with helper text "Malaysian phone number format: 60xxxxxxxxxx (required for payments)".
*   **Buttons:** "Save Changes" (currently disabled in light salmon).

### 28. Apply to be a Merchant Form
*   **Source File:** `Screenshot 2026-05-07 at 5.17.37 PM.png`
*   **Heading:** "Apply to be a Merchant (Fill out the form below to submit your business for review.)"
*   **On-Screen Fields & Placeholders:**
    *   Business Name text field: `e.g., My Local Store`
    *   Business Address multi-line text field: `e.g., 123 Main Street, City, Postcode`
    *   Phone Number text field: `e.g., +60123456789`
*   **Form Action Buttons:** "Submit Application" (active orange).

### 29. Security Settings (Change Password)
*   **Source File:** `Screenshot 2026-05-07 at 5.17.47 PM.png`
*   **Visual Assets:** Heading "Security Settings", subheading "Manage your account security preferences.", and a key icon.
*   **On-Screen Fields & Placeholders:**
    *   New Password text field: `Enter new password`
    *   Confirm New Password text field: `Confirm new password`
    *   Helper text at bottom: "Additional security features coming soon."
*   **Form Action Buttons:** "Change Password" (inactive light salmon).

### 30. Notifications Dashboard
*   **Source File:** `Screenshot 2026-05-07 at 5.17.58 PM.png`
*   **Unread Badging:** Heading "Notifications" with a blue circle badge containing the number `8`.
*   **Tab Filters:** Segmented bar displaying `All` (active, solid blue), `Requests`, `Accepted`, `Rejected`, and `New`.
*   **Utilities:** "Mark all as read" blue text button.
*   **Historical Activity Stream:**
    *   Row 1: "Payment Accepted" (green check icon, blue unread dot). Text: "Agile Technoprenuer Sdn Bhd accepted your payment request of RM200.00" | "6 minutes ago".
    *   Row 2: "Payment Accepted" (green check icon, blue unread dot). Text: "Agile Technoprenuer Sdn Bhd accepted your payment request of RM200.00" | "1 day ago".
    *   Row 3: "Payment Accepted" (green check icon, blue unread dot). Text: "Agile Technoprenuer Sdn Bhd accepted your payment request of RM30.00" | "2 days ago".
    *   Row 4: "Payment Rejected" (red warning icon, blue unread dot). Text: "Agile Technoprenuer Sdn Bhd rejected your payment request of RM20.00" | "2 days ago".
    *   Row 5: "Payment Accepted" (green check icon, blue unread dot). Text: "Agile Technoprenuer Sdn Bhd accepted your payment request of RM20.00" | "2 days ago".

### 31. Available Merchants (Map View - Main State)
*   **Source File:** `Screenshot 2026-05-07 at 5.18.21 PM.png`
*   **Map Control Interface:**
    *   Segmented top-right button "List View" (toggles back to list).
    *   Leaflet zoom controls `+` and `-` in the top left.
*   **Map Visualization:**
    *   Fully rendered street map centering around "Damansara Utama" (Selangor, Malaysia).
    *   Major shopping mall visual: "The Starling" clearly highlighted on the map.
    *   Red location drop pin representing the active merchant positioned on the map view.
    *   Attribution footer in the bottom right: "Leaflet | © OpenStreetMap contributors".

# Swimming Lesson Booking Test Plan
## Falkensteiner Family Hotel Diadora - Swimming Academy

### Test Overview
This test plan documents the complete user journey for booking a swimming lesson at Falkensteiner Resort Punta Skala's Swimming Academy. The test covers navigation from the homepage through to successful cart addition for two 21-month-old babies on September 14th.

### Test Prerequisites
- Browser: Chrome/Chromium
- Target URL: https://www.falkensteiner.com/en/family-hotel-diadora
- Test Data: 2 babies aged 21 months, booking date: September 14th, 2025

### Test Steps

#### Step 1: Navigate to Falkensteiner Homepage
1. **Action**: Navigate to `https://www.falkensteiner.com/en/family-hotel-diadora`
2. **Expected Result**: Falkensteiner homepage loads successfully
3. **Verification**: Page title contains "Falkensteiner" and main navigation is visible
4. **Screenshot**: `01-falkensteiner-homepage.png`

#### Step 2: Handle Cookie Consent
1. **Action**: Wait for cookie consent banner to appear
2. **Action**: Click "Accept All" or equivalent consent button
3. **Expected Result**: Cookie banner disappears, homepage content becomes fully accessible
4. **Verification**: Cookie banner is no longer visible, page interactions are enabled
5. **Screenshot**: `02-homepage-after-cookies.png`

#### Step 3: Navigate to Resort Punta Skala
1. **Action**: Look for Resort Punta Skala link/section on homepage
2. **Action**: Click on Resort Punta Skala link
3. **Expected Result**: Navigate to Resort Punta Skala specific page
4. **Verification**: URL contains "resortpuntaskala" and page shows resort-specific content
5. **Screenshot**: `03-resort-punta-skala-homepage.png`

#### Step 4: Access Swimming Academy via Camps and Academies
1. **Action**: Navigate to "Experience" section in main menu
2. **Action**: Click on "Camps and Academies" or similar link
3. **Expected Result**: Page displays various academy options including Swimming Academy
4. **Verification**: Swimming Academy card is visible with "Free of charge" pricing
5. **Screenshot**: `04-academies-page-with-swimming.png`

#### Step 5: Open Swimming Academy Booking Details
1. **Action**: Click on Swimming Academy card or "Reserve" button
2. **Expected Result**: Detailed Swimming Academy booking interface opens
3. **Verification**: 
   - Page shows Swimming Academy details
   - Age groups are visible (Baby Goldfish 6 months - 3 years old)
   - Booking form/calendar is accessible
4. **Screenshot**: `05-swimming-academy-booking-detail.png`

#### Step 6: Select Booking Date (September 14th)
1. **Action**: Click on date selector/calendar
2. **Action**: Navigate to September 2025 if not already visible
3. **Action**: Click on day "14" for September 14th
4. **Expected Result**: September 14th, 2025 is selected and highlighted
5. **Verification**: Date selector shows "14 Sep 2025" or equivalent
6. **Screenshot**: `06-swimming-academy-september-14-selected.png`

#### Step 7: Configure Age Group and Time Slot
1. **Action**: Verify "Baby Goldfish (6 months - 3 years old)" is appropriate for 21-month babies
2. **Action**: Select time slot (e.g., 09:30)
3. **Expected Result**: 
   - Appropriate age group is selected/highlighted
   - Time slot is selected (09:30-09:50 for 20-minute session)
4. **Verification**: Age group and time are displayed in booking summary

#### Step 8: Set Party Size for Two Babies
1. **Action**: Locate "Party size" dropdown/selector
2. **Action**: Click on party size dropdown
3. **Action**: Select "2" from dropdown options
4. **Expected Result**: Party size shows "2" participants
5. **Verification**: Booking summary reflects 2 participants
6. **Screenshot**: `07-swimming-lesson-ready-to-reserve.png`

#### Step 9: Complete Reservation (Add to Cart)
1. **Action**: Click "Reserve" button to add lesson to cart
2. **Expected Result**: Cart dialog/overlay appears showing booking details
3. **Verification**: 
   - Swimming Academy appears in cart
   - Date: 14 Sep 2025
   - Time: 09:30-09:50  
   - Price: €0.00 (free)
   - Timer shows time left to complete booking
4. **Screenshot**: `08-swimming-lesson-added-to-cart.png`

#### Step 10: Verify Successful Cart Addition
1. **Action**: Review cart contents
2. **Expected Result**: Cart shows complete booking details
3. **Verification Points**:
   - ✅ Swimming Academy lesson is listed
   - ✅ Correct date: September 14th, 2025
   - ✅ Correct time slot: 09:30-09:50
   - ✅ Correct duration: 20 minutes
   - ✅ Appropriate age group: Baby Goldfish (6mo-3yr)
   - ✅ Correct party size: 2 participants
   - ✅ Correct pricing: €0.00 (Free of charge)
   - ✅ Booking timer is active
   - ✅ "Change time or units" option available
   - ✅ "Add more experiences" option available
   - ✅ "Proceed" button available for checkout

### Test Data Summary
- **Website**: Falkensteiner Resort Punta Skala
- **Service**: Swimming Academy - Baby Goldfish Program
- **Target Age**: 21-month-old babies (fits 6 months - 3 years category)
- **Date**: September 14th, 2025
- **Time**: 09:30-09:50 (20 minutes)
- **Participants**: 2 babies
- **Cost**: Free of charge (€0.00)
- **Location**: Diadora indoor pool

### Key Business Rules Verified
1. **Age Appropriateness**: 21-month babies fit within "Baby Goldfish (6 months - 3 years old)" category
2. **Pricing**: Swimming Academy lessons are free of charge for hotel guests
3. **Duration**: Baby lessons are 20 minutes long
4. **Availability**: September 14th, 2025 has available slots
5. **Booking Process**: Multi-step process with date, time, and party size selection
6. **Cart Functionality**: Lessons can be added to cart with booking timer
7. **Cancellation Policy**: Fully refundable up until 24 hours before start time

### Expected Challenges & Solutions
- **Cookie Consent**: Handle privacy/cookie banners that may block interactions
- **Resort Navigation**: Navigate to correct resort (Punta Skala) rather than Family Hotel Diadora
- **Academy Discovery**: Find Swimming Academy through "Camps and Academies" section
- **Date Selection**: Navigate calendar interface to select specific date
- **Age Group Selection**: Understand age categories to select appropriate group
- **Form Interactions**: Handle dropdown selections and form field configurations

### Success Criteria
✅ Successfully navigated to Swimming Academy booking
✅ Selected appropriate age group for target demographic
✅ Configured booking for correct date and time
✅ Set party size to accommodate two babies
✅ Added swimming lesson to cart
✅ Verified all booking details are accurate
✅ Confirmed free pricing structure
✅ Demonstrated complete end-to-end booking flow

### Test Environment
- **Browser**: Chromium/Chrome
- **Viewport**: Full desktop view
- **Screenshots**: 8 comprehensive screenshots documenting each step
- **Network**: Standard connection (no offline scenarios)
- **Accessibility**: Page elements properly identified via accessibility tree

---
*Test plan generated based on actual booking session completed on January 8, 2025*

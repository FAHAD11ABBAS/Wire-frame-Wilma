# Wilma Platform - Student Absence Marking User Flow

## Project Overview
**Platform:** Wilma (Finnish school management system)  
**Feature:** Student self-reporting absence for the next day  
**Device:** Mobile (iOS/Android)  
**Wireframe Type:** Mid-fidelity  

---

## User Flow: Marking Absence for Next Day

### Step 1: Home Dashboard
**Screen:** Home Dashboard  
**User Action:** Student opens Wilma mobile app and logs in

**Elements:**
- Header with "Wilma" logo and user profile icon
- Student name displayed: "Matti Virtanen"
- Current date shown
- Main navigation menu with 4 options:
  - 📱 Etusivu (Home)
  - 📅 Poissaolot (Absences) ← **User selects this**
  - 💬 Viestit (Messages)
  - 📚 Lukujärjestys (Schedule)

**Interaction:** Tap on "Poissaolot" (Absences) button

---

### Step 2: Absences Overview
**Screen:** Absences Page  
**User Action:** View absence history and initiate new absence report

**Elements:**
- Header: "Poissaolot"
- Back button (←) to return to home
- Primary action button: "+ Ilmoita poissaolo" (Report absence) - Blue, prominent
- Absence history list showing:
  - Previous absence dates
  - Reasons for absence
  - Status (approved/pending)

**Interaction:** Tap on "+ Ilmoita poissaolo" button

---

### Step 3: Absence Report Form
**Screen:** Report Absence Form  
**User Action:** Fill in absence details for tomorrow

**Elements:**
- Header: "Ilmoita poissaolo" (Report Absence)
- Back button (←)
- Form fields:
  1. **Päivämäärä (Date):** 
     - Date picker showing tomorrow's date
     - Default: Next day (e.g., "11.12.2025")
  
  2. **Syy (Reason):**
     - Dropdown menu with options:
       - Sairaus (Illness)
       - Lääkäriaika (Doctor appointment)
       - Hammaslääkäriaika (Dentist appointment)
       - Muu syy (Other reason)
  
  3. **Lisätiedot (Additional Information):**
     - Text area for optional details
     - Placeholder: "Kerro tarvittaessa lisää..."

- Action buttons:
  - "Peruuta" (Cancel) - Gray, secondary
  - "Lähetä" (Submit) - Blue, primary

**Validation:**
- Date must be tomorrow or future date
- Reason must be selected
- Additional information is optional

**Interaction:** 
1. Select tomorrow's date
2. Choose reason from dropdown
3. Optionally add details
4. Tap "Lähetä" (Submit)

---

### Step 4: Confirmation
**Screen:** Success Confirmation  
**User Action:** View confirmation and return to home

**Elements:**
- Success icon: ✓ (Green checkmark)
- Confirmation message: "Poissaoloilmoitus lähetetty" (Absence notification sent)
- Summary of submitted information:
  - Date: 11.12.2025
  - Reason: Sairaus (Illness)
  - Additional info: (if provided)
- Note: "Huoltajalle lähetetty ilmoitus" (Guardian has been notified)
- Action button: "Palaa etusivulle" (Return to home) - Blue

**Interaction:** Tap "Palaa etusivulle" to return to dashboard

---

## Design Specifications

### Color Palette
- **Primary Blue:** #0066CC (buttons, links, active states)
- **Background Gray:** #F5F5F5 (page backgrounds)
- **White:** #FFFFFF (cards, form fields)
- **Text Black:** #333333 (primary text)
- **Text Gray:** #666666 (secondary text)
- **Success Green:** #28A745 (confirmation)
- **Border Gray:** #DDDDDD (dividers, borders)

### Typography
- **Headers:** 20px, Bold, Sans-serif
- **Body Text:** 16px, Regular, Sans-serif
- **Button Text:** 16px, Semi-bold, Sans-serif
- **Labels:** 14px, Regular, Sans-serif

### Spacing
- Screen padding: 16px
- Element spacing: 12px
- Button height: 48px
- Input field height: 44px

### Components
- **Buttons:** Rounded corners (8px), full width on mobile
- **Form fields:** Light border, rounded corners (4px)
- **Cards:** White background, subtle shadow
- **Navigation:** Bottom tab bar or hamburger menu

---

## User Journey Summary

1. **Entry Point:** Student opens Wilma app → Home Dashboard
2. **Navigation:** Taps "Poissaolot" (Absences)
3. **Action:** Taps "+ Ilmoita poissaolo" (Report absence)
4. **Input:** Fills form with tomorrow's date and reason
5. **Submission:** Taps "Lähetä" (Submit)
6. **Confirmation:** Views success message
7. **Exit:** Returns to home dashboard

**Total Steps:** 4 screens, approximately 30-60 seconds to complete

---

## Key Features

✅ **Simple Navigation:** Clear path from home to absence reporting  
✅ **Pre-filled Date:** Tomorrow's date suggested by default  
✅ **Dropdown Reasons:** Quick selection of common absence reasons  
✅ **Optional Details:** Flexibility to add more information  
✅ **Immediate Confirmation:** Clear feedback that submission was successful  
✅ **Guardian Notification:** Automatic notification sent to parent/guardian  

---

## Technical Considerations

### Accessibility
- High contrast text
- Touch targets minimum 44x44px
- Screen reader compatible labels
- Clear focus states

### Validation
- Date cannot be in the past
- Reason must be selected before submission
- Form shows error messages if validation fails

### Notifications
- Push notification confirmation to student
- Email/SMS notification to guardian
- In-app notification visible in Wilma

---

## Future Enhancements
- Multi-day absence selection
- Recurring absence patterns
- Attachment upload (e.g., doctor's note)
- Calendar view integration
- Absence statistics dashboard

---

**Document Version:** 1.0  
**Date:** December 10, 2025  
**Created for:** Wilma Platform Wireframe Assignment

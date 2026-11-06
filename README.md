# ChefChris-final-poe
# Chef Chris - Chef's Menu Manager
### MAST5112 - Portfolio of Evidence - Final POE

## Student Information
- **Name:** MANGANYI NTSAKELO LETELO
- **Student Number:** ST10529807
- **Module:** MAST5112 - Mobile Application Development
- **POE Part:** Final POE - Enhancing and Completing the Mobile Application
- **Institution:** IIE - The Independent Institute of Education
- **Submission Date:** 06 November 2026

## Project Description
Chef's Menu Manager is a React Native mobile application built for Chef Chris, a professional chef who wants to manage his restaurant menu digitally.

In Part 2, the app allowed the chef to add and view menu items. In this Final POE, the app has been enhanced to allow the chef to manage, search, filter, and analyse his full menu in one user-friendly app.

The app helps Chef Chris to:
- Keep track of all dishes across Starters, Main Courses and Desserts
- Quickly find a dish by name
- Update prices and descriptions when the menu changes
- See an overview of his menu with statistics

## Links
- **GitHub Repository:
- **Video Demonstration (YouTube)

> Replace the links above with your actual links before submitting.

## Features Implemented

### Part 2 Features (Carried Over)
- Clear application title: Chef Chris Menu Manager
- Input fields for Dish Name, Description, Course, and Price
- Save a menu item
- Display all menu items in a scrollable list
- Automatic update of list when a new item is added

### Final POE Features

#### 1. Manage Menu Items (25 Marks)
- **Edit an existing menu item:** Tap Edit on any card, form is pre-filled with that item's details
- **Update menu item information:** Change name, description, course or price and tap Update Item
- **Delete a menu item:** Tap Delete, confirmation Alert appears, item is removed immediately
- All changes are reflected immediately using React state `useState`

#### 2. Search and Filter Menu Items (20 Marks)
- **Search by name:** TextInput at top of list, filters in real-time (case-insensitive)
- **Filter by course:** Buttons - All, Starter, Main Course, Dessert
- **Clear search/filter:** "Clear Search & Filter - Show All" button resets both and shows all items
- Uses `useMemo` for efficient filtering

#### 3. Display Menu Statistics (20 Marks)
Displayed at the top in a clear card layout:
- **Total number of menu items**
- **Average price of all menu items** (calculated as sum / total, displayed as R XX.XX)
- **Number of items in each course:** Starters, Main Courses, Desserts
- Statistics update automatically when items are added, edited or deleted

#### 4. Enhance Application (20 Marks)
- **Reusable Component:** `MenuCard` - used for every item in the FlatList, handles display, Edit and Delete
- **Reusable Function:** `calculateStats(menuItems)` - calculates total, average, and per-course counts
- **Code Organisation:** Components, functions, state and styles are separated and clearly commented
- **Meaningful Names:** `dishName`, `handleSaveItem`, `filteredItems`, `handleDelete` etc.
- **Improved Validation:** Checks for empty fields, invalid price, price <= 0
- **Consistent Layout:** Same colours, spacing and card style throughout

#### 5. User Experience (10 Marks)
- **Easy to use:** Simple one-screen flow, large touch targets
- **Clear navigation:** Sections labelled - Statistics, Add Menu Item, Search & Filter, Menu Items
- **Meaningful messages:** Alert for "Validation Error", "Menu item added successfully!", "Menu item updated successfully!", "Confirm Delete"
- **Empty state message:** "No menu items have been added yet. Add your first dish!" or "No items match your search/filter."
- **Consistent look and feel:** Green #0a7a3e primary, orange for filter, white cards, same border radius throughout

## Technologies Used
- **Framework:** React Native with Expo
- **Language:** JavaScript (ES6)
- **Components:** View, Text, TextInput, TouchableOpacity, FlatList, ScrollView, Alert
- **State Management:** React Hooks - useState, useMemo
- **Styling:** React Native StyleSheet
- **Version Control:** Git & GitHub
- **Testing:** Expo Go on Android

## Colour Palette Explanation
| Colour | Hex | Usage |
| :--- | :--- | :--- |
| **Primary Green** | `#0a7a3e` | Title, Save button, prices, active course button - growth, freshness, food |
| **Accent Orange** | `#ff9800` | Filter buttons - energy, appetite |
| **Dark Grey** | `#1d1d1f` | Headings and body text |
| **Light Grey** | `#f8f9fa` | App background - clean kitchen feel |
| **White** | `#ffffff` | Cards and form - clean, readable |
| **Red** | `#d32f2f` | Delete button - danger / warning |
| **Blue** | `#1976d2` | Edit button - action |

## Project Structure

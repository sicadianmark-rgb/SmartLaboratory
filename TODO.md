# TODO: Implement Date Filtering for History Page

## Tasks:
- [x] Add state variables for single date and date range filters
- [x] Update the filters UI to include single date picker and FROM/TO date range pickers
- [x] Implement date filtering logic in the filteredHistory computation
- [x] Remove the old non-functional date input and filter button
- [x] Test the filtering functionality to ensure it works correctly
- [x] Update CSS if needed for the new date filter elements

## Details:
- Single date filter: Filters requests where the released date exactly matches the selected date
- Date range filter: Filters requests where the released date falls between the FROM and TO dates (inclusive)
- Filtering should be reactive - table updates automatically as dates are selected
- If both single date and range are set, prioritize single date filter
- If only FROM is set, filter from that date onwards
- If only TO is set, filter up to that date
- Dates are compared based on releasedDate field

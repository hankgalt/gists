Functional component based API data fetch and result rendering example with client side optimizations to improve user experience

- Implements search input debouncing using React.useEffect to avoid unnecessary API requests on input change.
- New MovieTiles functional component responsible for rendering resultset in movie tiles
    - implements pagination to reduce render time by limiting the number of movie tiles displayed while giving access to full dataset without refetching.
    - uses React.useMemo to preserve navigated subset for faster render on revisit.
- MovieTile component updated with data attribute and onClick navigation logic moved to MovieTiles component to avoid creating unnecessary onclick references for each of the MovieTile components.

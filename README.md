# Bus Route Estimator

A web application for visualizing bus routes and estimating arrival times. Upload Excel files containing route data, view routes on an interactive map, and get ETAs for stops.

## Features

- Upload Excel files containing route data
- Interactive map visualization of bus routes using OpenStreetMap
- Route selection via dropdown menu
- Stop information display
- ETA estimation (coming soon)

## Prerequisites

- Node.js (v14 or higher)
- npm (v6 or higher)

## Setup

1. Clone the repository:
```bash
git clone <repository-url>
cd bus-route-estimator
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```

## Excel File Format

The application expects Excel files with the following columns:
- RouteID: Unique identifier for the route
- StopName: Name of the bus stop
- Latitude: Stop's latitude coordinate
- Longitude: Stop's longitude coordinate
- StopTime: (Optional) Scheduled arrival time
- StopNumber: (Optional) Sequential number of the stop

Example Excel file structure:
```
RouteID,StopName,Latitude,Longitude,StopTime,StopNumber
R001,Main Terminal,40.7128,-74.0060,08:00,1
R001,City Center,40.7142,-74.0064,08:15,2
R001,University,40.7155,-74.0068,08:30,3
```

## Development

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

## Technologies Used

- React
- TypeScript
- Vite
- Leaflet.js (with OpenStreetMap)
- SheetJS (xlsx)
- Axios

## License

MIT 
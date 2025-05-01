# Delhi Metro Navigator

A Java application that helps users navigate the Delhi Metro transit system using graph algorithms to find optimal routes.

## 📝 Description

Delhi Metro Navigator is a console-based application that allows users to:
- View all stations in the Delhi Metro network
- Display the complete metro map 
- Find the shortest distance between stations
- Calculate the quickest travel time between stations
- Get detailed path information including interchanges

The application uses graph data structures and algorithms (Dijkstra's algorithm) to calculate optimal routes between stations, considering both distance and time factors.

## 🚇 Features

- **Station Listing:** View all available stations in the Delhi Metro network
- **Metro Map Visualization:** Display a text-based representation of the complete metro network
- **Multiple Input Methods:** Find stations by:
  - Serial number
  - Station code
  - Station name
- **Distance Optimization:** Calculate shortest distance routes between stations
- **Time Optimization:** Calculate fastest time routes between stations
- **Path Details:** Get comprehensive path information including:
  - Total distance
  - Total travel time
  - Number of interchanges required
  - Detailed station-by-station path

## 🧠 Algorithms & Data Structures

- **Graph Implementation:** Custom adjacency list representation using HashMap
- **Shortest Path:** Dijkstra's algorithm for optimal route calculation
- **Priority Queue:** Custom heap implementation for efficient path finding
- **Path Reconstruction:** Custom tracking of paths for detailed route information

## 🔍 Technical Implementation

The project consists of two main Java classes:
1. **Graph_M.java:** Contains the graph implementation, metro map creation, and all path finding algorithms
2. **Heap.java:** Implements a custom priority queue used by Dijkstra's algorithm

Key components include:
- Vertex representation with adjacency lists
- Edge representation with distance weights
- Line color tracking through station naming convention (using ~color suffix)
- Custom comparison logic for optimal path finding

## 🚀 Usage

1. Compile the Java files:
```
javac Graph_M.java Heap.java
```

2. Run the application:
```
java Graph_M
```

3. Follow the on-screen menu to:
   - List all stations
   - View the metro map
   - Find shortest paths by distance
   - Find shortest paths by time
   - Get detailed routing information

## 🗺️ Metro Line Information

The application includes information for the following Delhi Metro lines:
- Blue Line (B)
- Yellow Line (Y)
- Orange Line (O)
- Pink Line (P)
- Red Line (R)

Interchange stations are marked with multiple line identifiers (e.g., BY for Blue-Yellow interchange).

## 📊 Example

```
SOURCE STATION : Noida Sector 62~B
DESTINATION STATION : IGI Airport~O
DISTANCE : 28KM
NUMBER OF INTERCHANGES : 1
~~~~~~~~~~~~~
START  ==>  Noida Sector 62~B
Botanical Garden~B
Yamuna Bank~B
Rajiv Chowk~BY
New Delhi~YO
Shivaji Stadium~O
DDS Campus~O
IGI Airport~O   ==>    END
~~~~~~~~~~~~~
```

## 🛠️ Future Improvements

- Add a graphical user interface
- Include fare calculation
- Update with the latest Delhi Metro expansions
- Add real-time data integration
- Implement mobile applications

## 📄 License

This project is open-source and available under the MIT License.

---

Created by [Shanu Choudhary]

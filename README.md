# MMM-network-signal
adjust the icons and size to fit my own mirror

![Image of loading gif](https://raw.githubusercontent.com/Yuhan-1in/MMM-network-signal/master/loading.gif)

## Installation

cd ~/MagicMirror/modules
git clone https://github.com/Yuhan-1in/MMM-network-signal.git
cd MMM-network-signal
npm install

1. Clone this repo into `~/MagicMirror/modules` directory.
2. Install dependencies `npm i`
3. Configure your `~/MagicMirror/config/config.js`:

   ```
   {
       module: "MMM-network-signal",
       position: "bottom_right",
       config: {
           // Configuration of the module goes here
       }
   }
   ```

## Configuration Options

| **Option**         | **Default**                              | **Description**                         |
| ------------------ | ---------------------------------------- | --------------------------------------- |
| `updateInterval`   | `5000`                                   | Time in ms between connection tests     |
| `maxTimeout`       | `1000`                                   | Maximum timeout in ms for every pings   |
| `animationSpeed`   | `250`                                    | Icon change animation time in ms        |
| `initialLoadDelay` | `3000`                                   | Delay in ms for first ping              |
| `server`           | `8.8.8.8`                                | Pingable server IP address              |
| `thresholds`       | `{ strong: 50, medium: 150, weak: 500 }` | Tresholds for icons (ping answer in ms) |
| `showMessage`      | `true`                                   | Shows status messages depending on how good or bad is the connection |

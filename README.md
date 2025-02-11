# AI-Builders-Bootcamp-HW1
Build a Python Automation
"""
# BGP Live Stream Data Processing Notebook

## Description:
This Jupyter Notebook is designed to **subscribe to a real-time BGP (Border Gateway Protocol) feed** from the RiS internet exchange and , process the received 
messages, and store them in a structured Pandas DataFrame. It includes functionalities to:

- **Start, pause, and stop** the BGP data feed using interactive buttons.
- Convert **hex-encoded fields** to **ASCII** for human-readable format.
- Extract **useful features** from timestamps for **machine learning** applications.
- Save processed data as a **CSV file** for further analysis.
- Develop a 

## Features:
- Real-time WebSocket connection to RIS Live BGP data stream.
- Data parsing and transformation for easy analysis.
- Machine learning-ready time-based feature extraction.
- User-controlled streaming via Jupyter widgets.
- Preprocesses the dataframe for Useful Time-Series Analysis to figure out Trends in BGP updates over time. 
-ASN Contribution Analysis, to Identify major BGP route announcers. 
-Anomaly Detection, via monitoring Sudden spikes in withdrawals could indicate BGP attacks. 
-Feature Engineering for future ML models, is_weekend, hour, and announcement_count etc. are useful features.
-Main Goals for the Dashboard was as follows:

    -Track Routing Changes Over Time (Using the Time-Series Chart).
    -Analyze Autonomous Systen Numbers Contributions (Identify major BGP peering routers).
    -Detect Network Anomalies (Spike in withdrawals = possible route hijack).
  ## Usage:
1. Run the notebook.
2. Use the **Start button** to begin collecting BGP messages.
3. Use the **Pause button** to temporarily freeze processing.
4. Use the **Stop button** to stop the WebSocket stream.
5. Access collected data using `df_messages`.
6. Save data locally using `df_messages.to_csv("output.csv", index=False)`.

## Requirements:
- Python 3.x
- Libraries: `websocket-client`, `pandas`, `ipywidgets`, `datetime`
- Jupyter Notebook environment## Developer:
- **Author:** Shaji R. Nathan
- **Email:** shaji.nathan@ipinfusion.com
- **GitHub/Portfolio:** https://github.com/snathanfax/AI-Builders-Bootcamp-HW1

## License:
© 2025 [Shaji Ravindra. Nathan]. All rights reserved.
This program is free software: you can redistribute it and/or modify
it under the terms of the GNU Affero General Public License as published by the Free Software Foundation,
either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
See the GNU Affero General Public License for more details.

For details on GNU AGPLv3 licensing please, refer https://www.gnu.org/licenses/agpl-3.0.html.

## Version:
- **Date:** February 9, 2025
- **Version:** 1.0.0

"""

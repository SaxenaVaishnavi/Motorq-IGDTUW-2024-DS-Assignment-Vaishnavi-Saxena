# Motorq-IGDTUW-2024-DS-Assignment-Vaishnavi-Saxena

### Comparison Between Calculated Fuel Economy and Provided MPG:
- The calculated fuel economy for most vehicles either exceeds or falls short of the provided MPG values, indicating variability in real-world driving conditions.
- Vehicles like vehicle_3 and vehicle_5 showed a significantly higher calculated fuel economy compared to their provided MPG, suggesting they might be operating more efficiently under the given conditions.
- Conversely, vehicles like vehicle_4 and vehicle_9 have much lower calculated fuel economies than their provided MPG, possibly indicating inefficiencies, such as frequent idling, hard braking, stop-and-go traffic, or poor maintenance.

### Limitations and Considerations:
- Data Accuracy: The accuracy of the telemetry data and the assumptions made during calculations could introduce some level of error.
- Single Snapshot: The calculated fuel economy represents a snapshot over the period of data collection, and may not account for longer-term driving patterns or maintenance schedules.

### Assumptions
#### Missing Values Handling:
- Speed and Odometer: Missing values in the speed and odometer columns were handled using linear interpolation. This approach assumes that changes in speed and distance are continuous and that intermediate values can be estimated based on adjacent readings.
- Fuel Level: Missing values in the fuel level column were handled using forward fill (ffill), where the last observed fuel level was carried forward to fill gaps. This assumes that the fuel level remained constant until a new reading was recorded.

### Inferences:
#### Calculated vs. Provided Fuel Economy:
- The calculated fuel economy values varied significantly from the provided MPG values in some cases. This could be due to various factors such as differences in driving conditions, vehicle maintenance, or inaccuracies in sensor data.
- Vehicles with significantly higher or lower calculated fuel economy compared to the provided MPG might indicate potential discrepancies in the telemetry data or variations in actual driving behavior compared to standardized testing conditions.
- The interpolation and ffill methods used for handling missing data may have introduced some level of error, especially if there were long gaps between readings or sudden changes in vehicle performance that were not captured by the data.

### Conclusion:
The analysis provides valuable insights into the real-world fuel economy of different vehicles, helping to identify potential areas for improving fuel efficiency and reducing operational costs. Regular monitoring and comparison with provided MPG values can guide better decision-making for fleet management.

# Q38 – Smart Grid Fault Detection Optimization

## Course
Design and Analysis of Algorithms (DAA)

## Title
Smart Grid Fault Detection Optimization Using Pattern Detection

## Objective

To design an efficient pattern detection system that identifies abnormal patterns in smart-grid sensor data and analyze its efficiency, scalability, and contribution to power-system reliability.

## Approach

The program compares consecutive sensor readings.

The change is calculated as:

Change = |Current Reading - Previous Reading|

If the change exceeds the predefined threshold, a possible fault is detected.

## Detection Threshold

20.0

## Example

Input:

100 102 101 103 105 150 152 151

The change between 105 and 150 is:

45

Since 45 > 20, a possible fault is detected.

## Complexity

### Time Complexity
O(n)

### Extra Space Complexity
O(1)

## Important Constraints

- Real-time processing
- Sensor data accuracy
- Low computational overhead
- Scalability for large networks
- Fast fault detection

## Advantages

- Simple and fast.
- Suitable for streaming data.
- Linear time complexity.
- Low memory requirement.
- Can detect sudden anomalies quickly.

## Limitations

A fixed threshold may produce false positives due to sensor noise. Production systems can improve accuracy using filtering, statistical analysis, machine learning, and multi-sensor validation.

## Files

- `c_soucecode – C source code
- `Report.pdf` – Complete report
- `README.md` – Project documentation

## Result

The system successfully detects abnormal changes in smart-grid sensor readings. The proposed algorithm operates in O(n) time, making it suitable for real-time processing and scalable sensor monitoring.

## Conclusion

Efficient pattern detection can help identify power-grid faults quickly, reduce outage duration, protect equipment, and improve overall power-system reliability.

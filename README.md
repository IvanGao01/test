## SmartWatch Gesture

The SmartWatch Gestures Dataset has been collected to evaluate several gesture recognition algorithms for interacting with mobile applications using arm gestures.

Eight different users performed twenty repetitions of twenty different gestures, for a total of 3200 sequences. Each sequence contains acceleration data from the 3-axis accelerometer of a first generation Sony SmartWatch™, as well as timestamps from the different clock sources available on an Android device. The smartwatch was worn on the user's right wrist. The gestures have been manually segmented by the users performing them by tapping the smartwatch screen at the beginning and at the end of every repetition.

- Homepage: [https://tev.fbk.eu/resources/smartwatch](https://tev.fbk.eu/resources/smartwatch)
- Versions: 1.0.0
- Size: 5 MB
- Format: CSV
- Last Update: 2023-06-05

### Usage

```
\w 1
```

### Field Descriptions

| Colume      | Type      | Tag  | Original                   |
| ----------- | --------- | ---- | -------------------------- |
| time        | TIMESTAMP |      | System.currentTimeMillis() |
| time_nanos  | BIGINT    | NO   | System.nanoTime()          |
| time_event  | BIGINT    | NO   | event.timestamp            |
| access_x    | DOUBLE    | NO   | event.values[0]            |
| access_y    | DOUBLE    | NO   | event.values[1]            |
| access_z    | DOUBLE    | NO   | event.values[2]            |
| participant | STRING    | YES  |                            |
| gesture     | STRING    | YES  |                            |


<details>
  <summary>Click here to show/hide data</summary>

  <div style="overflow-x: auto;">
    <table>
      <thead>
        <tr>
          <th>time</th>
          <th>time_nanos</th>
          <th>time_event</th>
          <th>accel_x</th>
          <th>accel_y</th>
          <th>accel_z</th>
          <th>participant</th>
          <th>gesture</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>1384186054309</td>
          <td>78952598976553</td>
          <td>1452892000000</td>
          <td>1.532289</td>
          <td>-0.919373</td>
          <td>10.113108</td>
          <td>U01</td>
          <td>01</td>
        </tr>
        <tr>
          <td>1384186054419</td>
          <td>78952708778799</td>
          <td>1453002000000</td>
          <td>0.919373</td>
          <td>-0.919373</td>
          <td>9.959879</td>
          <td>U01</td>
          <td>01</td>
        </tr>
        <!-- 添加更多数据行 -->
      </tbody>
    </table>
  </div>
</details>

**Disclaimer: SmartWatch Gestures Dataset is provided for research or academic purposes only. Publications and works that use this dataset should please refer to one of the papers referenced below.**

### publications

- G. Costante, L. Porzi, O. Lanz, P. Valigi, E. Ricci, [Personalizing a Smartwatch-based Gesture Interface With Transfer Learning,](http://www.eurasip.org/Proceedings/Eusipco/Eusipco2014/HTML/papers/1569922319.pdf) 22nd European Signal Processing Conference, EUSIPCO 2014

- L. Porzi and S. Messelodi and C.M. Modena and E. Ricci: [A Smart Watch-based Gesture Recognition System for Assisting People with Visual Impairments.](https://dl.acm.org/doi/10.1145/2505483.2505487) ACM International Workshop on Interactive Multimedia on Mobile and Portable Devices  - IMMPD, Barcelona, Spain, 2013

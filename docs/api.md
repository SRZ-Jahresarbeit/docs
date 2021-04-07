## Data Consuming

Data is consumed via a rest api. The documentation can be found here:

```
https://raw.githubusercontent.com/SRZ-Jahresarbeit/docs/master/api-docs.json
```

To visualize the documentation, you can use [petstore.swagger.io](https://petstore.swagger.io/) and paste the above URL.

---

## Data Publishing

New data gets published via mqtt.
<br>
Use the topic `sensor/<id>` and the **payload** with your **measurement value**.

The payload can be any decimal value between <code>-2<sup>31</sup></code> and <code>2<sup>31</sup>-1</code>.
<br>
Keep in mind that the value is transmitted **without** any unit as a plain number and encoded as a string with `utf-8`!

#### Example

```
topic:
sensor/f658a3c1-d1cc-49d3-9976-ff2500b4187b

payload:
10.6
```

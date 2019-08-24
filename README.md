D3-Radial-Gauge
===============

D3.JS Radial Gauge / Multi Needle.

![alt tag](https://raw.githubusercontent.com/NickersWeb/D3-Radial-Gauge/master/SingleGauge.png)
![alt tag](https://raw.githubusercontent.com/NickersWeb/D3-Radial-Gauge/master/MultiGauge.png)

Here is the list of properties with their default value that can be changed according to your needs:

        {
               "ranges":[
                   {"id":"00b4c767-bc7b-4bea-9e56-229385ff75f8","min":0,"max":30,"thickness":0.5,"color":"#ff4f4f","value":"Severe"},
                   {"id":"62996c84-b822-4d02-aac7-3e7605bb173a","min":30,"max":50,"thickness":0.5,"color":"#ff8080","value":"Very Poor"},
                   {"id":"fc1664a4-8861-44d6-ac33-cb88fa54d683","min":50,"max":65,"thickness":0.5,"color":"#eaf424","value":"Poor"},
                   {"id":"42f4872d-0da8-489d-9236-a63d288026e2","min":65,"max":75,"thickness":0.5,"color":"#f5fa3d","value":"Fair"},
                   {"id":"970bb7e1-1f32-4aed-9e3e-1e4ea662458d","min":75,"max":90,"thickness":0.5,"color":"#269d2f","value":"Good"},
                   {"id":"6d399f34-5395-41fe-88ac-d557ea675069","min":90,"max":100,"thickness":0.5,"color":"#0ab80e","value":"Very Good"}
               ],
               "needles":[
                   {"id":"100aaf20-274d-4b64-99f4-e93de73f4fc1","value":100.0,"precision":1,"valueUnit":"ConditionofMainElementsAgeweighted","thickness":0.0,"color":"#416094","clickFunc":"","clickParams":""}
               ],
               "face":{"thickness":0.0},
               "format":null,
               "value":0.0,
               "valueUnit":"",
               "lowerLimit":0,
               "upperLimit":100,
               "step":10,
               "startAngle":0,
               "sweepAngle":180,
               "hasShadow":true,
               "autoScale":true,
               "showRanges":true,
               "isAnimated":true,
               "majorGradPrecision":1,
               "gaugeTitle":"Cond. Main+Age "
           };
 
Here is a usage sample:

    <div>
        <div id="svgTarget"></div>
    </div>
    <script>
        $(function () {
            var gaugeRanges = [
                {
                    From: 1.5,
                    To: 2.5,
                    Color: "#8DCB2A"
                }, {
                    From: 2.5,
                    To: 3.5,
                    Color: "#FFC700"
                }, {
                    From: 3.5,
                    To: 4.5,
                    Color: "#FF7A00"
                },
                {
                    From: 4.5,
                    To: 6,
                    Color: "#C20000"
                }];

            $("#svgTarget").mttD3Gauge({ data: gaugeRanges, value: 3 });
        });
    </script>

http://plnkr.co/edit/sP0dHuGoCpaIvCiqoNxF?p=preview

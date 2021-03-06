Javascript implementation of [Moshier's ephemeris](http://www.moshier.net) calculations for sun, planets, comets, asteroids and stars.

Initially written by [mivion](https://github.com/mivion/ephemeris), I converted it into a node module. I publish the module as a starting point for others, too. Pull requests welcome!

### Installation

`npm install ephemeris-node`

### Usage

*app.js*
```javascript
var ephemeris = require('ephemeris-moshier');

var result = ephemeris.getAllPlanets("10.08.2015 17:09:01", 10.0014, 53.5653, 0);

/* Check out the namespaces: date, observer and observed:

{ date:
   { gregorianTerrestrial: '10.8.2015 17:9:1',
     gregorianTerrestrialRaw:
      { day: 10,
        month: 8,
        year: 2015,
        hours: 17,
        minutes: 9,
        seconds: 1,
        julianDate: 2457244.5,
        julianTime: 0.7145949074074074,
        julian: 2457245.2145949076,
        j2000: 2015.6063370154895,
        b1950: 2015.6065478300004,
        j1900: 2015.6063370154895,
        delta: 68.01714323102905,
        terrestrial: 2457245.2145949076,
        universal: 2457245.2138076723,
        universalDate: [Object],
        universalDateString: '10.8.2015 17:7:52.983' },
     gregorianUniversal: '10.8.2015 17:7:52.983',
     gregorianDelta: '00:00:68.01714323102905',
     julianTerrestrial: 2457245.2145949076,
     julianUniversal: 2457245.2138076723,
     julianDelta: 0.0007872354540628362 },
  observer:
   { name: 'earth',
     longitueGeodetic: 10.0014,
     longitudeGeodecentric: 10.0014,
     latitudeGeodetic: 53.5653,
     latitudeGeodecentric: 53.38123133267187,
     heightGeodetic: 0,
     heightGeodecentric: 6364.336264644461 },
  observed:
   { sun:
      { name: 'sun',
        raw: [Object],
        apparentLongitudeDms30: '17°45\'39"',
        apparentLongitudeDms360: '137°45\'39"',
        apparentLongitudeDd: 137.76105855382917,
        geocentricDistanceKm: -1 },
     mercury:
      { name: 'mercury',
        raw: [Object],
        apparentLongitudeDms30: '5°2\'10"',
        apparentLongitudeDms360: '155°2\'10"',
        apparentLongitudeDd: 155.03637003916958,
        geocentricDistanceKm: -1 },
     venus:
      { name: 'venus',
        raw: [Object],
        apparentLongitudeDms30: '25°43\'16"',
        apparentLongitudeDms360: '145°43\'16"',
        apparentLongitudeDd: 145.7212923824036,
        geocentricDistanceKm: -1 },
     moon:
      { name: 'moon',
        raw: [Object],
        apparentLongitudeDms30: '2°41\'17"',
        apparentLongitudeDms360: '92°41\'17"',
        apparentLongitudeDd: 92.68823373136327,
        geocentricDistanceKm: 61.007764233212335 },
     mars:
      { name: 'mars',
        raw: [Object],
        apparentLongitudeDms30: '1°7\'20"',
        apparentLongitudeDms360: '121°7\'20"',
        apparentLongitudeDd: 121.12222806696656,
        geocentricDistanceKm: -1 },
     jupiter:
      { name: 'jupiter',
        raw: [Object],
        apparentLongitudeDms30: '29°50\'16"',
        apparentLongitudeDms360: '149°50\'16"',
        apparentLongitudeDd: 149.83799891400335,
        geocentricDistanceKm: -1 },
     saturn:
      { name: 'saturn',
        raw: [Object],
        apparentLongitudeDms30: '28°20\'25"',
        apparentLongitudeDms360: '238°20\'25"',
        apparentLongitudeDd: 238.34045318452542,
        geocentricDistanceKm: -1 },
     uranus:
      { name: 'uranus',
        raw: [Object],
        apparentLongitudeDms30: '20°24\'33"',
        apparentLongitudeDms360: '20°24\'33"',
        apparentLongitudeDd: 20.40921989582207,
        geocentricDistanceKm: -1 },
     neptune:
      { name: 'neptune',
        raw: [Object],
        apparentLongitudeDms30: '8°58\'37"',
        apparentLongitudeDms360: '338°58\'37"',
        apparentLongitudeDd: 338.9771304673532,
        geocentricDistanceKm: -1 },
     pluto:
      { name: 'pluto',
        raw: [Object],
        apparentLongitudeDms30: '13°27\'13"',
        apparentLongitudeDms360: '283°27\'13"',
        apparentLongitudeDd: 283.4537823191463,
        geocentricDistanceKm: -1 },
     chiron:
      { name: 'chiron',
        raw: [Object],
        apparentLongitudeDms30: '20°41\'58"',
        apparentLongitudeDms360: '350°41\'58"',
        apparentLongitudeDd: 350.6995558283406,
        geocentricDistanceKm: -1 },
     sirius:
      { name: 'sirius',
        raw: [Object],
        apparentLongitudeDms30: '11°27\'17"',
        apparentLongitudeDms360: '101°27\'17"',
        apparentLongitudeDd: 1.7707222368344282,
        geocentricDistanceKm: 7777 } } }
*/
```

### Contributers

This implementation based on code by [Steve Moshier](http://www.moshier.net).

The inital Javascript code has been written by [mivion](https://github.com/mivion/ephemeris).


### License

[GPL-2](http://www.gnu.org/licenses/gpl-2.0.html)

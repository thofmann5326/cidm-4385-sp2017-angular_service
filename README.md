# cidm4385-spring2017-angular_basics

This program is made to take a metric or imperial number and convert them to the opisite format.

## Features

* Allow user to input a number
* Allow user to select the converstion from and too
* do this for Mass/Wieght, Length, and volume convertions


## Code Example

The 'Code' is not complete due to the lack of time to input all converstion formulas:
Volume convertsion as an example:
```
<h2>Volume Convert</h2>
		
		<div ng-controller="UnitConverterController as ucc">
			<input type="text" ng-model="ucc.lengthValue" id="Length_value" name="VALUE" placeholder="Enter amount">
            <select ng-model="ucc.selected_metric_volume_unit" 
                    ng-options="unit.unit_name for unit in ucc.metric_volume_units" 
                    ng-change="ucc.showSelectedUnit()"></select>
            <select ng-model="ucc.selected_imperial_volume_unit" 
                    ng-options="unit.unit_name for unit in ucc.imperial_volume_units" 
                    ng-change="ucc.showSelectedUnit()"></select>
			
			<!--<select>-->
			<div>
				<p>Selected unit is: <span ng-bind="ucc.selected_metric_volume_unit.unit_name"></span></p>
				<p>Selected unit is: <span ng-bind="ucc.selected_imperial_volume_unit.unit_name"></span></p>
			</div>
		</div>
```

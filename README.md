# disney-exercise
assignment
<html>
	<head>
		<title>Assignment</title>
		<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular.min.js"></script>
		<script type="text/javascript" src="https://code.angularjs.org/1.3.15/angular-route.min.js"></script>
		<script type="text/javascript" src="js/index.js"></script>
		<style>
			.leftBlock , .rightBlock {
				float: left;
				border: 2px solid;
				margin: 5px;
				height: 500px;
			}
			.leftBlock {
				width: 200px;
			}
			.rightBlock {
				width: 500px;
			}
			li {
				list-style: none;
				cursor: pointer;
			}
			li:hover {
				text-decoration: underline;
			}
		</style>
	</head>
	<body ng-app="myApp" ng-controller="myController">
		<div>
			Assignment
		</div>
		<div class="leftBlock">
			<ul>
				<li ng-click="showMain()">
					Main Page
				</li>
				<li ng-click="showForm()">
					Form Page
				</li>
				<li ng-click="showResource()">
					Resources
				</li>
			</ul>
		</div>
		<div ng-view class="rightBlock">
		</div>
	</body>
</html>

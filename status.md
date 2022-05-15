#### Initial Setup According to documentation
- First setup without any major tweaking is [here](https://youtu.be/iaAuGmnUBi8)


#### Test 2 (25 April) -
- Changed Cartographer params
- Changed Navigation params
- Made a world model in Gazebo for tests
- Video - [here](https://youtu.be/0duuqKgF_pc)

#### Test 3 (29 April) -
- taken refrence randy's pull on mavros code
- Used mavlink_router and replaced rviz by Mission planner
- Tested flow of SET_POSITION_TARGET_GLOBAL_INT messages from gcs to navigation package

#### Currently - proper testing and Fixing problems in this [Pull](https://github.com/mavlink/mavros/pull/1184)
made changes (suggested by voon) that includes 
implementing that as a separate plugin and using different name ( used offboard target name instead of setpoint_target)
implemented that plugin in mavros_extras
##### NOTE: (not yet pushed the changes) due to a bug that causing diffrent modes to trigger from the given command for eg: auto mode going to steering, guided changes to HOLD etc.

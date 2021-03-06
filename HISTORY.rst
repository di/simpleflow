Changelog
---------

0.12.1
~~~~~~

- Don't override passed "default" in json_dumps() (#155)
- Expose activity context (#156)

0.12.0
~~~~~~

- Improve process management (#142)

0.11.17
~~~~~~~

- Don't reap children in the back of multiprocessing (#141)
- Don't force to pass a workflow to activity workers (#133)
- Don't override the task list if not standalone (#139)
- Split FuncGroup submit (#146)
- CI: Test on python 3 (#144)
- Decider: use workflow's task list if unset (#148)

0.11.16
~~~~~~~

- Refactor: cleanups and many python 3 compatibility issues fixed (#135)
- Introduce AggregationException to inspect exceptions inside canvas.Group/Chain (#92)
- Improve heartbeating, now enabled by default on activity workers (#136)

0.11.15
~~~~~~~

- Fix tag_list declaration in case no tag is associated with the workflow
- Fix listing workflow tasks not handling "scheduled" (not started) tasks correctly
- Fix CSV formatter outputing an extra "None" at the end of the output
- Fix 'simpleflow activity.rerun' resolving the bad function name if not the last event

0.11.14
~~~~~~~

- Various little fixes around process management, heartbeat, logging (#110)

0.11.13
~~~~~~~

- Add ability to provide a 'run ID' with 'simpleflow standalone --repair'

0.11.12
~~~~~~~

- Fix --tags argument for simpleflow standalone (#114)
- Improve tests and add integration tests (#116)
- Add 'simpleflow activity.rerun' command (#117)

0.11.11
~~~~~~~

- Fix a circular import on simpleflow.swf.executor

0.11.10
~~~~~~~

- Fix previous_history initialization (#106)
- Improve WorkflowExecutionQueryset default date values (#111)

0.11.9
~~~~~~

- Add a --repair option to simpleflow standalone (#100)

0.11.8
~~~~~~

- Retry boto.swf connection to avoid frequent errors when using IAM roles (#99)

0.11.7
~~~~~~

Same as 0.11.6 but the 0.11.6 on pypi is broken (pushed something similar to 0.11.5 by mistake)

0.11.6
~~~~~~

- Add issubclass_ method (#96)
- Avoid duplicate logs if root logger has an handler (#97)
- Allow passing SWF domain via the SWF_DOMAIN environment variable (#98)

0.11.5
~~~~~~

- Don't mask activity cancel exception (#84)
- Propagate all decision response attributes up to Executor.replay() (#76, #94)

0.11.4
~~~~~~

- ISO dates in workflow history #91
- Fix potential infinite retry loop #90

0.11.3
~~~~~~

- Fix replay hooks introduced in 0.11.2 (#86)
- Remove python3 compatibility from README (which was not working for a long time)

0.11.2
~~~~~~

- Add new workflow hooks (#79)

0.11.1
~~~~~~

- Fix logging when an exception occurs

0.11.0
~~~~~~

- Merge ``swf`` package into simplefow for easier maintenance.


0.10.4 and below
~~~~~~~~~~~~~~~~

Sorry changes were not documented for simpleflow <= 0.10.x.

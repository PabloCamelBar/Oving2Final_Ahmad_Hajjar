Lastet prosjektet opp på github som public.
konfigurert workflow med actions på git, med java with maven.
lagt til build og testsource i pom.xml filen, for å kjøre testene når man puller/pusher til git.

siden testene har både tester som gir true og false så vil vi få feilmelding i builden:




/////////////////////////////////////////////////////////////////////////////////////
Error:  Failures: 
Error:    isLeapYearTest.testIfDevidableBy100AndNot400:72 expected: <false> but was: <true>
Error:    isLeapYearTest.testIfDevidableBy400:57 expected: <true> but was: <false>
Error:    isLeapYearTest.testIfNotDividableBy4:67 expected: <false> but was: <true>
[INFO] 
Error:  Tests run: 7, Failures: 3, Errors: 0, Skipped: 0
[INFO] 
[INFO] ------------------------------------------------------------------------
[INFO] BUILD FAILURE
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  9.067 s
[INFO] Finished at: 2023-10-25T07:25:45Z
[INFO] ------------------------------------------------------------------------
Error:  Failed to execute goal org.apache.maven.plugins:maven-surefire-plugin:3.1.2:test (default-test) on project Oving2Final: There are test failures.
Error:  
Error:  Please refer to /home/runner/work/Oving2Final_Ahmad_Hajjar/Oving2Final_Ahmad_Hajjar/target/surefire-reports for the individual test results.
Error:  Please refer to dump files (if any exist) [date].dump, [date]-jvmRun[N].dump and [date].dumpstream.
Error:  -> [Help 1]
Error:  
Error:  To see the full stack trace of the errors, re-run Maven with the -e switch.
Error:  Re-run Maven using the -X switch to enable full debug logging.
Error:  
Error:  For more information about the errors and possible solutions, please read the following articles:
Error:  [Help 1] http://cwiki.apache.org/confluence/display/MAVEN/MojoFailureException
Error: Process completed with exit code 1.
///////////////////////////////////////////////////////////////////////////////////

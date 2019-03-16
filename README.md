# java_modules

javac -d bin --module-source-path src/ --module com.atul

java --module-path bin --module com.atul/com.atul.TestModule

jar -c --file=bin/com.atul.jar --main-class=com.atul.TestModule -C bin/com.atul .

java -jar bin/com.atul.jar

jlink --module-path "bin;C:\Program Files\Java\jdk-11.0.2\jmods" --add-modules com.atul --output out-standalone

bin/java --module com.atul/com.atul.TestModule
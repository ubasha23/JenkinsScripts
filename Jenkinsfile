
node 

{


def maven_home;


stage ("checkout the source code")

{

git 'https://github.com/ubasha23/course.git'

maven_home= tool 'Maven3'

}


stage ("compiling source code")

{

sh "'${maven_home}/bin/mvn' compile"

}
stage ("testing source code")

{

sh "'${maven_home}/bin/mvn' test"

}
stage ("building artifact")

{

sh "'${maven_home}/bin/mvn' package"

}


}
# Butler Wiki

Welcome to the ansible-role-butler wiki!

## How to download and configure the butler.

```text
wget https://s3.us-east-1.amazonaws.com/butlercli/1.0.0/linux/butler
chmod +x butler
mv butler /usr/local/bin/
```

## Command to export plugins.

```text
butler plugins export --server localhost:8080 --username admin --password admin
```

```text
+------------------------------------+-----------+--------------------------------+
|                NAME                |  VERSION  |          DESCRIPTION           |
+------------------------------------+-----------+--------------------------------+
| jdk-tool                           |       1.2 | JDK Tool Plugin                |
| script-security                    |      1.51 | Script Security Plugin         |
| cloudbees-folder                   |       6.7 | Folders Plugin                 |
| command-launcher                   |       1.3 | Command Agent Launcher Plugin  |
| jackson2-api                       | 2.9.8     | Jackson 2 API Plugin           |
| github-api                         |      1.95 | GitHub API Plugin              |
| structs                            |      1.17 | Structs Plugin                 |
| workflow-step-api                  |      2.18 | Pipeline: Step API             |
| git-server                         |       1.7 | Jenkins GIT server Plugin      |
| workflow-scm-step                  |       2.7 | Pipeline: SCM Step             |
| workflow-cps-global-lib            |      2.12 | Pipeline: Shared Groovy        |
|                                    |           | Libraries                      |
| bouncycastle-api                   |      2.17 | bouncycastle API Plugin        |
| javadoc                            |       1.4 | Javadoc Plugin                 |
| credentials                        | 2.1.18    | Credentials Plugin             |
| variant                            |       1.1 | Variant Plugin                 |
| apache-httpcomponents-client-4-api | 4.5.5-3.0 | Jenkins Apache HttpComponents  |
|                                    |           | Client 4.x API Plugin          |
| ssh-credentials                    |      1.14 | SSH Credentials Plugin         |
| favorite                           | 2.3.2     | Favorite                       |
| jsch                               | 0.1.55    | Jenkins JSch dependency plugin |
| git-client                         | 2.7.6     | Jenkins Git client plugin      |
| maven-plugin                       |       3.2 | Maven Integration plugin       |
| scm-api                            | 2.3.0     | SCM API Plugin                 |
| display-url-api                    | 2.3.0     | Display URL API                |
| run-condition                      |       1.2 | Run Condition Plugin           |
| mailer                             |      1.23 | Jenkins Mailer Plugin          |
| workflow-api                       |      2.33 | Pipeline: API                  |
| junit                              | 1.26.1    | JUnit Plugin                   |
| branch-api                         | 2.1.2     | Branch API Plugin              |
| matrix-project                     |      1.13 | Matrix Project Plugin          |
| git                                | 3.9.2     | Jenkins Git plugin             |
| jquery                             | 1.12.4-0  | jQuery plugin                  |
| token-macro                        |       2.6 | Token Macro Plugin             |
| plain-credentials                  |       1.5 | Plain Credentials Plugin       |
| blueocean-rest                     | 1.10.2    | REST API for Blue Ocean        |
| github                             | 1.29.3    | GitHub plugin                  |
| workflow-multibranch               |      2.20 | Pipeline: Multibranch          |
| workflow-basic-steps               |      2.14 | Pipeline: Basic Steps          |
| pipeline-milestone-step            | 1.3.1     | Pipeline: Milestone Step       |
| authentication-tokens              |       1.3 | Authentication Tokens API      |
|                                    |           | Plugin                         |
| jquery-detached                    | 1.2.1     | JavaScript GUI Lib: jQuery     |
|                                    |           | bundles (jQuery and jQuery UI) |
|                                    |           | plugin                         |
| ace-editor                         |       1.1 | JavaScript GUI Lib: ACE Editor |
|                                    |           | bundle plugin                  |
| workflow-support                   |       3.1 | Pipeline: Supporting APIs      |
| workflow-cps                       |      2.62 | Pipeline: Groovy               |
| pipeline-input-step                |       2.9 | Pipeline: Input Step           |
| docker-commons                     |      1.13 | Docker Commons Plugin          |
| pipeline-stage-step                |       2.3 | Pipeline: Stage Step           |
| workflow-job                       |      2.31 | Pipeline: Job                  |
| handlebars                         | 1.1.1     | JavaScript GUI Lib: Handlebars |
|                                    |           | bundle plugin                  |
| pipeline-graph-analysis            |       1.9 | Pipeline Graph Analysis Plugin |
| pipeline-rest-api                  |      2.10 | Pipeline: REST API Plugin      |
| momentjs                           | 1.1.1     | JavaScript GUI Lib: Moment.js  |
|                                    |           | bundle plugin                  |
| durable-task                       |      1.28 | Durable Task Plugin            |
| pipeline-stage-view                |      2.10 | Pipeline: Stage View Plugin    |
| pipeline-build-step                |       2.7 | Pipeline: Build Step           |
| credentials-binding                |      1.17 | Credentials Binding Plugin     |
| docker-workflow                    |      1.17 | Docker Pipeline                |
| pipeline-model-api                 | 1.3.4.1   | Pipeline: Model API            |
| pubsub-light                       |      1.12 | Jenkins Pub-Sub "light" Bus    |
| pipeline-model-extensions          | 1.3.4.1   | Pipeline: Declarative          |
|                                    |           | Extension Points API           |
| sse-gateway                        |      1.17 | Server Sent Events (SSE)       |
|                                    |           | Gateway Plugin                 |
| workflow-durable-task-step         |      2.28 | Pipeline: Nodes and Processes  |
| pipeline-stage-tags-metadata       | 1.3.4.1   | Pipeline: Stage Tags Metadata  |
| pipeline-model-declarative-agent   | 1.1.1     | Pipeline: Declarative Agent    |
|                                    |           | API                            |
| blueocean-events                   | 1.10.2    | Events API for Blue Ocean      |
| pipeline-model-definition          | 1.3.4.1   | Pipeline: Declarative          |
| lockable-resources                 |       2.4 | Lockable Resources plugin      |
| workflow-aggregator                |       2.6 | Pipeline                       |
| docker-slaves                      | 1.0.7     | Docker Slaves Plugin           |
| github-branch-source               | 2.4.2     | GitHub Branch Source Plugin    |
| pipeline-githubnotify-step         | 1.0.4     | Pipeline GitHub Notify Step    |
|                                    |           | Plugin                         |
| blueocean-i18n                     | 1.10.2    | i18n for Blue Ocean            |
| conditional-buildstep              | 1.3.6     | Conditional BuildStep          |
| parameterized-trigger              | 2.35.2    | Jenkins Parameterized Trigger  |
|                                    |           | plugin                         |
| blueocean-autofavorite             | 1.2.3     | Autofavorite for Blue Ocean    |
| build-pipeline-plugin              | 1.5.8     | Build Pipeline Plugin          |
| simple-travis-runner               |       1.0 | Simple Travis Pipeline Runner  |
|                                    |           | Plugin                         |
| serenity                           |       1.2 | Jenkins Serenity plugin        |
| pipeline-utility-steps             | 2.2.0     | Pipeline Utility Steps         |
| email-ext                          |      2.63 | Email Extension Plugin         |
| blueocean-commons                  | 1.10.2    | Common API for Blue Ocean      |
| blueocean                          | 1.10.2    | Blue Ocean                     |
| blueocean-pipeline-scm-api         | 1.10.2    | Pipeline SCM API for Blue      |
|                                    |           | Ocean                          |
| htmlpublisher                      |      1.18 | HTML Publisher plugin          |
| jenkins-design-language            | 1.10.2    | Jenkins Design Language        |
| windows-slaves                     |       1.4 | WMI Windows Agents Plugin      |
| blueocean-core-js                  | 1.10.2    | Blue Ocean Core JS             |
| blueocean-web                      | 1.10.2    | Web for Blue Ocean             |
| matrix-auth                        |       2.3 | Matrix Authorization Strategy  |
|                                    |           | Plugin                         |
| blueocean-jwt                      | 1.10.2    | JWT for Blue Ocean             |
| blueocean-rest-impl                | 1.10.2    | REST Implementation for Blue   |
|                                    |           | Ocean                          |
| ssh-slaves                         | 1.29.4    | Jenkins SSH Slaves plugin      |
| blueocean-pipeline-api-impl        | 1.10.2    | Pipeline implementation for    |
|                                    |           | Blue Ocean                     |
| blueocean-dashboard                | 1.10.2    | Dashboard for Blue Ocean       |
| blueocean-pipeline-editor          | 1.10.2    | Blue Ocean Pipeline Editor     |
| docker-java-api                    | 3.0.14    | Docker API Plugin              |
| blueocean-github-pipeline          | 1.10.2    | GitHub Pipeline for Blue Ocean |
| blueocean-git-pipeline             | 1.10.2    | Git Pipeline for Blue Ocean    |
| job-direct-mail                    |       1.5 | Job Direct Mail Plugin         |
| blueocean-config                   | 1.10.2    | Config API for Blue Ocean      |
| mapdb-api                          | 1.0.9.0   | MapDB API Plugin               |
| mercurial                          |       2.5 | Jenkins Mercurial plugin       |
| docker-plugin                      | 1.1.5     | Docker plugin                  |
| handy-uri-templates-2-api          | 2.1.6-1.0 | Handy Uri Templates 2.x API    |
|                                    |           | Plugin                         |
| blueocean-display-url              | 2.2.0     | Display URL for Blue Ocean     |
| cloudbees-bitbucket-branch-source  | 2.4.0     | Bitbucket Branch Source Plugin |
| blueocean-bitbucket-pipeline       | 1.10.2    | Bitbucket Pipeline for Blue    |
|                                    |           | Ocean                          |
| docker-swarm                       |       1.6 | Docker Swarm Plugin            |
| blueocean-personalization          | 1.10.2    | Personalization for Blue Ocean |
| jira                               | 3.0.5     | Jenkins JIRA plugin            |
| blueocean-jira                     | 1.10.2    | JIRA Integration for Blue      |
|                                    |           | Ocean                          |
| docker-compose-build-step          |       1.0 | Docker Compose Build Step      |
|                                    |           | Plugin                         |
| antisamy-markup-formatter          |       1.5 | OWASP Markup Formatter Plugin  |
| subversion                         | 2.12.1    | Jenkins Subversion Plug-in     |
| pom2config                         |       1.2 | pom2config                     |
| poll-mailbox-trigger-plugin        |     1.026 | Poll Mailbox Trigger Plugin    |
| icon-shim                          | 2.0.3     | Icon Shim Plugin               |
| github-pullrequest                 | 0.2.4     | GitHub Integration Plugin      |
| emailext-template                  |       1.1 | Email Extension Template       |
|                                    |           | Plugin                         |
| code-coverage-api                  | 1.0.7     | Code Coverage API Plugin       |
| cobertura                          |      1.13 | Jenkins Cobertura Plugin       |
| ant                                |       1.9 | Ant Plugin                     |
| pam-auth                           |       1.4 | PAM Authentication plugin      |
| ldap                               |      1.20 | LDAP Plugin                    |
| external-monitor-job               |       1.7 | External Monitor Job Type      |
|                                    |           | Plugin                         |
| codecover                          |       1.1 | Jenkins CodeCover plugin       |
| github-coverage-reporter           |       1.1 | Github Coverage Reporter       |
| github-pr-coverage-status          | 2.0.0     | GitHub Pull Request Coverage   |
|                                    |           | Status                         |
| codebeamer-coverage-publisher      |       1.2 | Codebeamer Coverage Publisher  |
|                                    |           | Plugin                         |
| unique-id                          | 2.1.3     | Unique ID Library Plugin       |
| urbancode-velocity                 | 2.0.1     | UrbanCode Velocity Plugin      |
| ibm-cloud-devops                   | 2.0.6     | IBM Cloud DevOps               |
| covcomplplot                       | 1.1.1     | Coverage/Complexity Scatter    |
|                                    |           | Plot PlugIn                    |
| audit-trail                        |       2.4 | Audit Trail                    |
+------------------------------------+-----------+--------------------------------+
```

It will create a file with name _**plugins.txt**_

```text
[root@c09e20219c3a /]# cat plugins.txt 
jdk-tool@1.2
script-security@1.51
cloudbees-folder@6.7
command-launcher@1.3
jackson2-api@2.9.8
github-api@1.95
structs@1.17
workflow-step-api@2.18
git-server@1.7
workflow-scm-step@2.7
workflow-cps-global-lib@2.12
bouncycastle-api@2.17
javadoc@1.4
credentials@2.1.18
variant@1.1
apache-httpcomponents-client-4-api@4.5.5-3.0
ssh-credentials@1.14
favorite@2.3.2
jsch@0.1.55
git-client@2.7.6
maven-plugin@3.2
scm-api@2.3.0
display-url-api@2.3.0
run-condition@1.2
mailer@1.23
workflow-api@2.33
junit@1.26.1
branch-api@2.1.2
matrix-project@1.13
git@3.9.2
jquery@1.12.4-0
token-macro@2.6
plain-credentials@1.5
blueocean-rest@1.10.2
github@1.29.3
workflow-multibranch@2.20
workflow-basic-steps@2.14
pipeline-milestone-step@1.3.1
authentication-tokens@1.3
jquery-detached@1.2.1
ace-editor@1.1
workflow-support@3.1
workflow-cps@2.62
pipeline-input-step@2.9
docker-commons@1.13
pipeline-stage-step@2.3
workflow-job@2.31
handlebars@1.1.1
pipeline-graph-analysis@1.9
pipeline-rest-api@2.10
momentjs@1.1.1
durable-task@1.28
pipeline-stage-view@2.10
pipeline-build-step@2.7
credentials-binding@1.17
docker-workflow@1.17
pipeline-model-api@1.3.4.1
pubsub-light@1.12
pipeline-model-extensions@1.3.4.1
sse-gateway@1.17
workflow-durable-task-step@2.28
pipeline-stage-tags-metadata@1.3.4.1
pipeline-model-declarative-agent@1.1.1
blueocean-events@1.10.2
pipeline-model-definition@1.3.4.1
lockable-resources@2.4
workflow-aggregator@2.6
docker-slaves@1.0.7
github-branch-source@2.4.2
pipeline-githubnotify-step@1.0.4
blueocean-i18n@1.10.2
conditional-buildstep@1.3.6
parameterized-trigger@2.35.2
blueocean-autofavorite@1.2.3
build-pipeline-plugin@1.5.8
simple-travis-runner@1.0
serenity@1.2
pipeline-utility-steps@2.2.0
email-ext@2.63
blueocean-commons@1.10.2
blueocean@1.10.2
blueocean-pipeline-scm-api@1.10.2
htmlpublisher@1.18
jenkins-design-language@1.10.2
windows-slaves@1.4
blueocean-core-js@1.10.2
blueocean-web@1.10.2
matrix-auth@2.3
blueocean-jwt@1.10.2
blueocean-rest-impl@1.10.2
ssh-slaves@1.29.4
blueocean-pipeline-api-impl@1.10.2
blueocean-dashboard@1.10.2
blueocean-pipeline-editor@1.10.2
docker-java-api@3.0.14
blueocean-github-pipeline@1.10.2
blueocean-git-pipeline@1.10.2
job-direct-mail@1.5
blueocean-config@1.10.2
mapdb-api@1.0.9.0
mercurial@2.5
docker-plugin@1.1.5
handy-uri-templates-2-api@2.1.6-1.0
blueocean-display-url@2.2.0
cloudbees-bitbucket-branch-source@2.4.0
blueocean-bitbucket-pipeline@1.10.2
docker-swarm@1.6
blueocean-personalization@1.10.2
jira@3.0.5
blueocean-jira@1.10.2
docker-compose-build-step@1.0
antisamy-markup-formatter@1.5
subversion@2.12.1
pom2config@1.2
poll-mailbox-trigger-plugin@1.026
icon-shim@2.0.3
github-pullrequest@0.2.4
emailext-template@1.1
code-coverage-api@1.0.7
cobertura@1.13
ant@1.9
pam-auth@1.4
ldap@1.20
external-monitor-job@1.7
codecover@1.1
github-coverage-reporter@1.1
github-pr-coverage-status@2.0.0
codebeamer-coverage-publisher@1.2
unique-id@2.1.3
urbancode-velocity@2.0.1
ibm-cloud-devops@2.0.6
covcomplplot@1.1.1
audit-trail@2.4
```

## Command to import plugins.

_**Note:**_ Before import make sure you have file with name _**plugins.txt**_

```text
butler plugins import --server localhost:8080 --username admin --password admin
```

## Command to export jobs.

```text
[root@c09e20219c3a /]# butler jobs export --server localhost:8080 --username admin --password admin
Exporting job: Fibonocci-CPP
```

It will create folder with name: _**jobs**_

```text
[root@c09e20219c3a /]# tree jobs
jobs
└── Fibonocci-CPP
    └── config.xml

1 directory, 1 file
```

## Command to import jobs.

_**Note:**_ Before import make sure you have folder with name _**jobs**_

```text
[root@c09e20219c3a /]# butler jobs import --server localhost:8080 --username admin --password admin
```

**Source:** [https://github.com/mlabouardy/butler/blob/master/README.md](https://github.com/mlabouardy/butler/blob/master/README.md)


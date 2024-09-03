[myawesometmlsolution1] Operating Details
====================================

.. important::
   These are the operating details for your TML solution.

.. tip::
   You must have your [myawesometmlsolution1] container running before connecting to the Visualization and Airflow URLs.

.. list-table::

   * - **Type**
     - **Details**
     - **Explanation**
   * - TML Solution Studio Docker Run Command
     - `docker run -d \-\-net=host \-\-env MAINHOST=127.0.0.1 \-\-env AIRFLOWPORT=9000 -v <change to your local folder>:/dagslocalbackup:z -v /var/run/docker.sock:/var/run/docker.sock:z \-\-env GITREPOURL=https://github.com/<Enter Github username>/raspberrypi.git \-\-env CHIP=AMD64 \-\-env TSS=1 \-\-env SOLUTIONNAME=TSS \-\-env READTHEDOCS=<Enter your readthedocs token> \-\-env  GITUSERNAME=<Enter your Github username> \-\-env GITPASSWORD=<Enter personal access token> \-\-env DOCKERUSERNAME=<Enter Dockerhub username> \-\-env DOCKERPASSWORD=<Enter your docker hub password> maadsdocker/tml-solution- studio-with-airflow-amd64`
     - This is the TML Solution Studio Docker Run command.  

       Note for MAC users change amd64 to arm64 in 

       the container name. 
   * - Your Solution Docker Container
     - maadsdocker/myawesometmlsolution1-amd64 (https://hub.docker.com/r/maadsdocker/myawesometmlsolution1-amd64)
     - This is the name of your solution container
   * - Your Solution Docker Run Command
     - docker run -d \-\-net=host \-\-env TSS=0 \-\-env SOLUTIONNAME=TSS \-\-env GITUSERNAME=smaurice101 

\-\-env GITPASSWORD=<Enter Github Password>  \-\-env GITREPOURL=https://github.com/smaurice101/raspberrypi.git 

\-\-env READTHEDOCS=<Enter Readthedocs token> maadsdocker/myawesometmlsolution1-amd64


     - This is the Docker Run command for your 

       solution container.  Note ports may change at runtime. 

       The solution documentation will update automatically.
   * - Visualization URL
     - http://localhost:43447/dashboard.html?topic=iot-preprocess-data&offset=-1&groupid=&rollbackoffset=500&topictype=prediction&append=0&secure=1
     - This is the visualization URL for your 

       TML dashboard. Note ports may change at runtime. 

       The solution documentation will update automatically.
   * - Solution Airflow URL
     - http://localhost:9000
     - This is the Airflow URL for your solution container.  

       NOTE: While this is provided in the container - you 

       should run/schedule solution containerss from the TSS
   * - [myawesometmlsolution1] Github Repo
     - https://github.com/smaurice101/raspberrypi/tree/main/tml-airflow/dags/tml-solutions/myawesometmlsolution1
     - This is the Github repo for all your solution code
   * - Readthedocs URL
     - https://myawesometmlsolution1.readthedocs.io
     - This is this url.
   * - Solution Trigger DAG
     - None
     - This is the name of the solution DAG you 

       chose to trigger 
   * - TML Binaries Listening Ports
     - VIPERHOST_PRODUCE=127.0.1.1, VIPERPORT_PRODUCE=38715, VIPERHOST_PREPOCESS=127.0.1.1, VIPERPORT_PREPROCESS=44005, VIPERHOST_ML=127.0.1.1, VIPERPORT_ML=38951, VIPERHOST_PREDCT=127.0.1.1, VIPERPORT_PREDICT=46679, HPDEHOST=127.0.1.1, HPDEPORT=33833, HPDEHOST_PREDICT=127.0.1.1, HPDEPORT_PREDICT=40149
     - These are the ports the TML binaries 

       are listening on.
   * - TMUX Windows
     - python-produce-7622-myawesometmlsolution1, python-preprocess-516-myawesometmlsolution1, viper-produce, viper-preprocess, viper-ml, viper-predict
     - Your solution is running in these  

       TMUX windows:
   
        - To view windows, type:

          **tmux ls**

        - To go inside window, type:

          **tmux a -t <window name>**

        - To exit window, type:

          **CTLR+b, d**

        - To scroll window, type:

          **CTLR+b, [**

        - To un-scroll window, type:

          **CTLR+[**

       

FROM launcher.gcr.io/google/debian10
RUN apt update && apt upgrade
RUN apt install -y curl git zip unzip xz-utils file
RUN git clone https://github.com/flutter/flutter.git -b stable
ENV PATH $PATH:/flutter/bin
RUN flutter config --no-analytics
RUN flutter upgrade
ENTRYPOINT ["flutter"]
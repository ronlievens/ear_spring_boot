# Basis image met Open Liberty
FROM open-liberty:kernel-slim

# Kopieer server config en EAR
COPY server.xml /config/
COPY target/deployable.ear /config/apps/

# Stel working directory
WORKDIR /config

# Open Liberty startscript
CMD ["/opt/ibm/wlp/bin/server", "run", "defaultServer"]

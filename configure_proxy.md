Para configurar proxy en la compu,




---- Fish configs
para crear un alias en fish:
    - alias proxyon="export http_proxy=http://proxy.cab.cnea.gov.ar:3128/ && export https_proxy=http://proxy.cab.cnea.gov.ar:3128/ && env {http,https}_proxy=http://proxy.cab.cnea.gov.ar:3128"
    - funcsave proxyon

django-cms
==========

To deploy on HPE Helion Stackato, execute the following command:

     cf push --no-start
     cf create-service <postgresql-service-name> default django-cms-db
     cf bind-service django-cms django-cms-db
     cf restart django-cms

The default username and password is `demo`

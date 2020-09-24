Lesson4 -- > Lets check the Services on Consul
==============================================

Agenda

1. Copy the Consul UI IP address from the output command

2. Open a browser and issue http://Consul_ip

 .. image:: /_static/consul_ui.png

3. You can see that we have 5 service shown in the consul UI

    ```app1_update```
 
    ```app2```

    ```bigip_tgw```

    ```consul```

    ```microapp1```

4. Service ```microapp1``` is running in the Consul Connect Service Mesh, service ```app1_update``` & ```app2``` are  the service running behind the BIG-IP. Service ```bigip_tgw``` is the terminating gateway service registered to the Consul Connect

5. You can check all the services by issuing ```cd /home/udf/consul-tg-env/service-configs```

6. All these services were created by doing ```make all`` in lesson3

7. Click on each service in the Consul UI to learn more about it

8. Click on the ```microapp1-->Service_check-->Proxy Info``` to see that Connect Sidecar Listening is failing


 .. image:: /_static/proxyfail.png

.. note:: You can verify that the Connect Sidecar is showing Red in Proxy Health

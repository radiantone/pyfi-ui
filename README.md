![flow1](./screens/pyfi.svg)

NodeJS/Vue UI for PYFI

PYFI will be a fully distributed open and extensible platform for building Nifi-like computation and data orchestration networks on top of a transactional & reliable enterprise message broker technology. In addition, it will have persistence of network data metrics and computational results in an enterprise data (e.g. SQL) warehouse.

The architecture for PYFI is illustrated below, but one of the key themes vs Apache Nifi is PYFI's separation of underlying messaging & persistent queues from the UI. In PYFI, processors are queue data consumers that scale, in a fully distributed way, across a network - as first class citizens. This prevents them from cannibalizing resources in a VM where they would otherwise be mutexed against other processors (such as in Nifi). Higher levels of performance, scaling and reliability are achieved with this design.

Another key theme in PYFI will be the dynamic scripting of processors and full transparency of processor behaviors. Making this a runtime feature means you don't have to endure complex and lengthy modifications to low-level source code, builds and redeploys. In an enterprise, that cycle can be frought with hurdles and approvals that prevent needed changes from coming quickly - not to mention dependency and versioning issues. PYFI avoids all that by creating a highly observable compute platform that doesn't compromise on security or features.

Lastly (for now), PYFI UI is built using industry modern javascript frameworks on top of NodeJS. This allows the UI to be extended with any type of javascript/typescript or VueJS component from the vast Node/Javascript ecosystem - integrating well with widgets from other apps inside an enterprise.

**Sponsoring**

This project is very exciting and will raise the bar for dynamic, observable distributed data flow systems. The technology is already out there and matured but needs to be brought together as a whole. This project is seeking intrepid sponsors would want access to the unpacked, unminimized source code and direct influence over integrations and designs going forward. Please let me know if you want to join in this vision!

![flow1](./screens/pyfi1.png)
![flow1](./screens/architecture2.png)
![flow1](./screens/architecture3.png)

To run:

$ python -m http.server 8000

Then point your browser to http://localhost:8000

NOTE: If you are on a smaller screen computer (e.g. like a macbook or something) you might need to reduce the scaling of your browser from 100% to 90-80% for the UI to render correctly.


![flow2](./screens/pyfi7.png)
![flow2](./screens/pyfi2.png)
![flow3](./screens/pyfi3.png)
![flow4](./screens/pyfi4.png)
![flow6](./screens/pyfi6.png)
![flow6](./screens/screen14.png)
![flow6](./screens/screen15.png)
![flow6](./screens/screen16.png)

架构说明
=================

.. image:: _static/img/structure.png
    :alt: 组件架构图


组件说明
=================

Glance
`````````````
现指 Glance 管理后台，是核心组件（Core）, 使用 Django Class Based View 风格开发，支持 Restful API。

`Github <https://github.com/glance/glance.git>`_


Coco
````````
实现了 SSH Server 和 Web Terminal Server 的组件，提供 SSH 和 WebSocket 接口, 使用 Paramiko 和 Flask 开发。


`Github <https://github.com/glance/coco.git>`__


Luna
````````
现在是 Web Terminal 前端，计划前端页面都由该项目提供，Glance 只提供 API，不再负责后台渲染html等。

`Github <https://github.com/glance/luna.git>`__


Guacamole
```````````
Apache 跳板机项目，Glance 使用其组件实现 RDP 功能，Glance 并没有修改其代码而是添加了额外的插件，支持 Glance 调用。


Glance-Python-SDK
```````````````````````
Glance API Python SDK，Coco 目前使用该 SDK 与 Glance API 交互。

`Github <https://github.com/glance/glance-python-sdk.git>`__



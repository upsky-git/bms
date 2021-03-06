# 查询SSH密钥列表（OpenStack原生）<a name="ZH-CN_TOPIC_0060384658"></a>

## 功能介绍<a name="section17769131"></a>

查询SSH密钥信息列表。

## 约束<a name="section25186711103718"></a>

不支持分页查询。

## URI<a name="section40393097103718"></a>

GET /v2.1/\{project\_id\}/os-keypairs

参数说明请参见[表1](#table875418115417)。

**表 1**  参数说明

<a name="table875418115417"></a>
<table><thead align="left"><tr id="row20751518135416"><th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.1"><p id="p67050730103718"><a name="p67050730103718"></a><a name="p67050730103718"></a>参数</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.2"><p id="p62400032103718"><a name="p62400032103718"></a><a name="p62400032103718"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="33.33333333333333%" id="mcps1.2.4.1.3"><p id="p21237868103718"><a name="p21237868103718"></a><a name="p21237868103718"></a>描述</p>
</th>
</tr>
</thead>
<tbody><tr id="row675161812542"><td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.1 "><p id="p23650911103718"><a name="p23650911103718"></a><a name="p23650911103718"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.2 "><p id="p36675672103718"><a name="p36675672103718"></a><a name="p36675672103718"></a>是</p>
</td>
<td class="cellrowborder" valign="top" width="33.33333333333333%" headers="mcps1.2.4.1.3 "><p id="p17939461103718"><a name="p17939461103718"></a><a name="p17939461103718"></a>项目ID。</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section43810255103718"></a>

不涉及。

## 响应消息<a name="section60965769103718"></a>

-   响应参数

    <a name="table27586210103718"></a>
    <table><thead align="left"><tr id="row41984926103718"><th class="cellrowborder" valign="top" width="22.48224822482248%" id="mcps1.1.4.1.1"><p id="p19987085"><a name="p19987085"></a><a name="p19987085"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.722872287228725%" id="mcps1.1.4.1.2"><p id="p4546697"><a name="p4546697"></a><a name="p4546697"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.7948794879488%" id="mcps1.1.4.1.3"><p id="p32738149"><a name="p32738149"></a><a name="p32738149"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row30149674103718"><td class="cellrowborder" valign="top" width="22.48224822482248%" headers="mcps1.1.4.1.1 "><p id="p26204567103718"><a name="p26204567103718"></a><a name="p26204567103718"></a>keypairs</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.722872287228725%" headers="mcps1.1.4.1.2 "><p id="p42195172103718"><a name="p42195172103718"></a><a name="p42195172103718"></a>列表数据结构，参见“[1] keypairs字段数据结构说明”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.7948794879488%" headers="mcps1.1.4.1.3 "><p id="p62365753103718"><a name="p62365753103718"></a><a name="p62365753103718"></a>密钥信息列表。</p>
    </td>
    </tr>
    </tbody>
    </table>

    \[1\] keypairs字段数据结构说明

    <a name="table31933500103718"></a>
    <table><thead align="left"><tr id="row13327014103718"><th class="cellrowborder" valign="top" width="22.509999999999998%" id="mcps1.1.4.1.1"><p id="p898483610238"><a name="p898483610238"></a><a name="p898483610238"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.77%" id="mcps1.1.4.1.2"><p id="p398620365236"><a name="p398620365236"></a><a name="p398620365236"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.72%" id="mcps1.1.4.1.3"><p id="p69881436202319"><a name="p69881436202319"></a><a name="p69881436202319"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row65555086103718"><td class="cellrowborder" valign="top" width="22.509999999999998%" headers="mcps1.1.4.1.1 "><p id="p8361735103718"><a name="p8361735103718"></a><a name="p8361735103718"></a>keypair</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.77%" headers="mcps1.1.4.1.2 "><p id="p6211933103718"><a name="p6211933103718"></a><a name="p6211933103718"></a>字典数据结构，参见“[2] keypair字段数据结构说明”。</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.72%" headers="mcps1.1.4.1.3 "><p id="p33404535103718"><a name="p33404535103718"></a><a name="p33404535103718"></a>密钥信息详情。</p>
    </td>
    </tr>
    </tbody>
    </table>

    \[2\] keypair字段数据结构说明

    <a name="table58497453103718"></a>
    <table><thead align="left"><tr id="row32349076103718"><th class="cellrowborder" valign="top" width="22.830000000000002%" id="mcps1.1.4.1.1"><p id="p97199488231"><a name="p97199488231"></a><a name="p97199488231"></a>参数</p>
    </th>
    <th class="cellrowborder" valign="top" width="28.89%" id="mcps1.1.4.1.2"><p id="p20720548142312"><a name="p20720548142312"></a><a name="p20720548142312"></a>参数类型</p>
    </th>
    <th class="cellrowborder" valign="top" width="48.28%" id="mcps1.1.4.1.3"><p id="p14724548132319"><a name="p14724548132319"></a><a name="p14724548132319"></a>描述</p>
    </th>
    </tr>
    </thead>
    <tbody><tr id="row45087230103718"><td class="cellrowborder" valign="top" width="22.830000000000002%" headers="mcps1.1.4.1.1 "><p id="p28187038103718"><a name="p28187038103718"></a><a name="p28187038103718"></a>fingerprint</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.89%" headers="mcps1.1.4.1.2 "><p id="p1448759103718"><a name="p1448759103718"></a><a name="p1448759103718"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.28%" headers="mcps1.1.4.1.3 "><p id="p50240624103718"><a name="p50240624103718"></a><a name="p50240624103718"></a>密钥对应指纹信息。</p>
    </td>
    </tr>
    <tr id="row49512432103718"><td class="cellrowborder" valign="top" width="22.830000000000002%" headers="mcps1.1.4.1.1 "><p id="p51084028103718"><a name="p51084028103718"></a><a name="p51084028103718"></a>name</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.89%" headers="mcps1.1.4.1.2 "><p id="p44165629103718"><a name="p44165629103718"></a><a name="p44165629103718"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.28%" headers="mcps1.1.4.1.3 "><p id="p20646235103718"><a name="p20646235103718"></a><a name="p20646235103718"></a>密钥名称。</p>
    </td>
    </tr>
    <tr id="row51598392103718"><td class="cellrowborder" valign="top" width="22.830000000000002%" headers="mcps1.1.4.1.1 "><p id="p18720236103718"><a name="p18720236103718"></a><a name="p18720236103718"></a>public_key</p>
    </td>
    <td class="cellrowborder" valign="top" width="28.89%" headers="mcps1.1.4.1.2 "><p id="p39944111103718"><a name="p39944111103718"></a><a name="p39944111103718"></a>String</p>
    </td>
    <td class="cellrowborder" valign="top" width="48.28%" headers="mcps1.1.4.1.3 "><p id="p14247596103718"><a name="p14247596103718"></a><a name="p14247596103718"></a>密钥对应publicKey信息。</p>
    </td>
    </tr>
    </tbody>
    </table>


-   响应样例

    ```
    {
        "keypairs": [
            {
                "keypair": {
                    "fingerprint": "15:b0:f8:b3:f9:48:63:71:cf:7b:5b:38:6d:44:2d:4a",
                    "name": "keypair-601a2305-4f25-41ed-89c6-2a966fc8027a",
                    "public_key": "ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAAAgQC+Eo/RZRngaGTkFs7I62ZjsIlO79KklKbMXi8F+KITD4bVQHHn+kV+4gRgkgCRbdoDqoGfpaDFs877DYX9n4z6FrAIZ4PES8TNKhatifpn9NdQYWA+IkU8CuvlEKGuFpKRi/k7JLos/gHi2hy7QUwgtRvcefvD/vgQZOVw/mGR9Q== Generated-by-Nova"
                }
            }
        ]
    }
    ```


## 返回值<a name="section29598436103718"></a>

请参考[通用返回值](通用返回值.md)。


# SpreadJS-计量检定模块

在现代计量领域，计量检定（又称计量器具强制检定）是量值传递的一种重要形式，用于评定计量器具的计量性能，确定其量值是否准确一致，实现手段包括计量检验、出具检定证书和加封盖印等。我国计量检定机构众多，但管理体制仍相对落后，信息化水平、技术水平参差不齐，重复建设严重。为了不断提高计量检定与校准的自动化水平，实现实时分析任务完成情况、自动生成台帐报表和有效跟踪记录工作数据，基于 B/S 架构的新一代计量检定系统正在逐步替代传统检定方式，旨在形成更为快速、高效、安全的计量检定体系。

葡萄城表格技术以 纯前端表格控件 SpreadJS 和 服务端表格组件 GcExcel 为核心组件，可用于构建新一代计量检定系统，完善计量器具的模板管理模块，扩展检定证书的生成功能，使系统检定证书的生成效率和标准达到或超过计量检定院的专业要求。


![输入图片说明](https://videos.grapecity.com.cn/SpreadJS/online/%E8%AE%A1%E9%87%8F%E6%A3%80%E5%AE%9A.mp4)

## 开发计量检定模块的技术难点

### 模板管理：自动化程度低，模板设计器功能单一

- 传统的模板管理方式无法自定义函数，难以灵活调用表单数据
- 设计器功能单一，实现检定、校准和不合格通知书的标准模板的难度大
- 系统扩展能力不足，不能修改现有函数规则和模板内容，后期维护成本高
- 权限控制难，业务人员无法自主编制模板，并提交核验
- 模板复用性差，不能实时编辑计算公式，修改检定证书结果区域的呈现方式

### 证书管理：检定证书无法智能生成

- 系统无法在线生成证书，不能根据计量器具自动填充检定结果
- 用户在线编辑检定证书的结果时需要额外安装第三方插件
- 系统无法将标准模板与检定结果区域合并，形成完整的检定证书
- 证书管理不能满足用户精准打印、特殊字符或多页打印的需求
- 系统不支持批量证书更新以及批量打印等功能

###  葡萄城表格技术的优势

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E8%AE%A1%E9%87%8F%E6%A3%80%E5%AE%9A%E6%9E%B6%E6%9E%84%E5%9B%BE.png)

 **#### 实现前端填报，简化证书设计流程** 
借助 SpreadJS，可直接在 B/S 系统中设计出类似 Excel 和 Word 样式的证书模板，并直接使用 Excel 的计算公式，也可自定义行业专属公式。SpreadJS 提供的设计器可同时满足在线设计、编辑和打印等功能，以此为基础，可快速搭建出一系列专业的业务模块，如输入值勘误、自动化设备对接和自动生成图表。

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%871.png)

 **#### 提高证书模板复用性，降低维护成本** 
SpreadJS 提供了高度类似 Excel 的功能，业务人员无需专门学习模板设计器的使用，也不需要开发人员介入，便可自行完成模板的修改。借助 SpreadJS 的 API（如拷贝粘贴、富文本编辑、公式编辑、条件格式、页面设置、数据验证、数据绑定和图表等）可开发出更多定制化选项，丰富证书模板的呈现形式，提高模板复用性，降低后期维护成本。

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%872.png)

 **#### 降低权限控制的开发难度** 

在模板数据填报过程中，需要根据业务需求控制不同区域的填报权限，传统的方式难以控制用户行为，而借助 SpreadJS 只需少量代码便可以实现权限控制。
![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%873.png)

 **#### 提供更加精准的证书打印样式** 
计量检定证书对于模板文字的大小样式、字体以及特殊字符的要求十分严苛，借助 SpreadJS ，可以在打印或模板输出时设置分页，以满足多页打印的需求。

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%874.png)

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%875.png)

 **#### 满足批量导出证书模板的需求** 
借助服务端表格组件 GcExcel，可以在后台将证书批量导出为 PDF，解决批量证书更新以及批量打印的需求，减轻浏览器压力，实现大文件存储备份的需求。

![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/spreadjs/industry/measure/%E5%9B%BE%E7%89%876.png)

### 葡萄城表格技术的功能特色

 **支持跨平台开发** 
以原生方式嵌入，支持 B/S、H5 小程序、APP 和桌面应用程序开发

 **支持国产操作系统** 
支持 Windows、Mac、Linux，通过麒麟软件、统信 UOS 兼容性认证

 **不依赖第三方库** 
加载、编辑、导入、导出 Excel 时无需预装插件和第三方应用软件

 **支持云应用开发** 
支持公有云部署、私有云部署和独立服务器部署

 **支持主流技术栈** 
前端组件基于 HTML5 标准，可与前、后端技术框架相结合

 **开放的 API 接口** 
内置大量 API 接口可供调用，轻松扩展，满足更多定制化需求

### 葡萄城表格技术的成功案例

 **大庆金桥 - 计量器具检定证书的生成与打印** 
借助 SpreadJS 可不用安装任何插件，便可创建并导入支持 Excel 公式的台帐报表模板，方便检定机构管理台帐和统计信息，并可衔接连贯系统内各项业务，为计量管理工作提供有力支持。
[![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/casestudies/casestudies-dqjq/pic05.png)](https://www.grapecity.com.cn/developer/casestudies/dqjq)

 **鲸控仪器 - 某计量检测云平台** 

通过对 SpreadJS 二次开发，检测云平台实现了证书模板的在线编辑设计，简化了数据绑定的实现难度，让用户使用起来更加方便。

[![输入图片说明](https://www.grapecity.com.cn/images/metalsmith/developer/casestudies/casestudies-jkyq/pic06.png)](https://www.grapecity.com.cn/developer/casestudies/jkyq)

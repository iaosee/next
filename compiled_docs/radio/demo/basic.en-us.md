{"title":"Basic Usage","meta":{"title":"Basic Usage","description":"\n"},"codes":{"jsx":"import { Radio } from '@alifd/next';\n\nReactDOM.render((\n    <div>\n        <h4>Without Label</h4>\n        <Radio defaultChecked />&nbsp;\n        <Radio checked />&nbsp;\n        <Radio disabled />&nbsp;\n        <Radio checked disabled />&nbsp;\n        <Radio />\n        <br />\n        <h4>With Label</h4>\n        <Radio id=\"apple\">Apple</Radio>&nbsp;\n        <Radio id=\"banana\" /><label htmlFor=\"banana\" className=\"next-radio-label\">Banana</label>&nbsp;\n        <Radio id=\"apple2\" label=\"Apple\" className=\"testClassname\" />\n    </div>\n), mountNode);\n"},"body":"\n````jsx\nimport { Radio } from '@alifd/next';\n\nReactDOM.render((\n    <div>\n        <h4>Without Label</h4>\n        <Radio defaultChecked />&nbsp;\n        <Radio checked />&nbsp;\n        <Radio disabled />&nbsp;\n        <Radio checked disabled />&nbsp;\n        <Radio />\n        <br />\n        <h4>With Label</h4>\n        <Radio id=\"apple\">Apple</Radio>&nbsp;\n        <Radio id=\"banana\" /><label htmlFor=\"banana\" className=\"next-radio-label\">Banana</label>&nbsp;\n        <Radio id=\"apple2\" label=\"Apple\" className=\"testClassname\" />\n    </div>\n), mountNode);\n````","html":"<script>(function(){\"use strict\";\n\nvar _next = require(\"@alifd/next\");\n\nReactDOM.render(React.createElement(\n    \"div\",\n    null,\n    React.createElement(\n        \"h4\",\n        null,\n        \"Without Label\"\n    ),\n    React.createElement(_next.Radio, { defaultChecked: true }),\n    \"\\xA0\",\n    React.createElement(_next.Radio, { checked: true }),\n    \"\\xA0\",\n    React.createElement(_next.Radio, { disabled: true }),\n    \"\\xA0\",\n    React.createElement(_next.Radio, { checked: true, disabled: true }),\n    \"\\xA0\",\n    React.createElement(_next.Radio, null),\n    React.createElement(\"br\", null),\n    React.createElement(\n        \"h4\",\n        null,\n        \"With Label\"\n    ),\n    React.createElement(\n        _next.Radio,\n        { id: \"apple\" },\n        \"Apple\"\n    ),\n    \"\\xA0\",\n    React.createElement(_next.Radio, { id: \"banana\" }),\n    React.createElement(\n        \"label\",\n        { htmlFor: \"banana\", className: \"next-radio-label\" },\n        \"Banana\"\n    ),\n    \"\\xA0\",\n    React.createElement(_next.Radio, { id: \"apple2\", label: \"Apple\", className: \"testClassname\" })\n), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> Radio <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">(</span>\n    <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>div</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>h4</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Without Label</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>h4</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">defaultChecked</span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">checked</span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">disabled</span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">checked</span> <span class=\"token attr-name\">disabled</span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>br</span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>h4</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">With Label</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>h4</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">id</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>apple<span class=\"token punctuation\">\"</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Apple</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span><span class=\"token class-name\">Radio</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">id</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>banana<span class=\"token punctuation\">\"</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span>label</span> <span class=\"token attr-name\">htmlFor</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>banana<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">className</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>next-radio-label<span class=\"token punctuation\">\"</span></span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">Banana</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>label</span><span class=\"token punctuation\">></span></span><span class=\"token plain-text\">&amp;nbsp;\n        </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Radio</span></span> <span class=\"token attr-name\">id</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>apple2<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">label</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>Apple<span class=\"token punctuation\">\"</span></span> <span class=\"token attr-name\">className</span><span class=\"token attr-value\"><span class=\"token punctuation attr-equals\">=</span><span class=\"token punctuation\">\"</span>testClassname<span class=\"token punctuation\">\"</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token plain-text\">\n    </span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;/</span>div</span><span class=\"token punctuation\">></span></span>\n<span class=\"token punctuation\">)</span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>"}
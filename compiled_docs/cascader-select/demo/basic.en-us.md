{"title":"Basic Usage","meta":{"title":"Basic Usage","description":"\n<p>Demo the basic single select usage.</p>\n","order":"0"},"codes":{"jsx":"import { CascaderSelect } from '@alifd/next';\n\nclass Demo extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            data: []\n        };\n    }\n\n    componentDidMount() {\n        fetch('https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json')\n            .then(response => response.json())\n            .then(data => {\n                this.setState({ data });\n            })\n            .catch(e => console.log(e));\n    }\n\n    handleChange = (value, data, extra) => {\n        console.log(value, data, extra);\n    }\n\n    render() {\n        return <CascaderSelect dataSource={this.state.data} onChange={this.handleChange} />;\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n"},"body":"\n````jsx\nimport { CascaderSelect } from '@alifd/next';\n\nclass Demo extends React.Component {\n    constructor(props) {\n        super(props);\n\n        this.state = {\n            data: []\n        };\n    }\n\n    componentDidMount() {\n        fetch('https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json')\n            .then(response => response.json())\n            .then(data => {\n                this.setState({ data });\n            })\n            .catch(e => console.log(e));\n    }\n\n    handleChange = (value, data, extra) => {\n        console.log(value, data, extra);\n    }\n\n    render() {\n        return <CascaderSelect dataSource={this.state.data} onChange={this.handleChange} />;\n    }\n}\n\nReactDOM.render(<Demo />, mountNode);\n````","name":"basic","html":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nvar Demo = function (_React$Component) {\n    _inherits(Demo, _React$Component);\n\n    function Demo(props) {\n        _classCallCheck(this, Demo);\n\n        var _this = _possibleConstructorReturn(this, (Demo.__proto__ || Object.getPrototypeOf(Demo)).call(this, props));\n\n        _this.handleChange = function (value, data, extra) {\n            console.log(value, data, extra);\n        };\n\n        _this.state = {\n            data: []\n        };\n        return _this;\n    }\n\n    _createClass(Demo, [{\n        key: 'componentDidMount',\n        value: function componentDidMount() {\n            var _this2 = this;\n\n            fetch('https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json').then(function (response) {\n                return response.json();\n            }).then(function (data) {\n                _this2.setState({ data: data });\n            }).catch(function (e) {\n                return console.log(e);\n            });\n        }\n    }, {\n        key: 'render',\n        value: function render() {\n            return React.createElement(_next.CascaderSelect, { dataSource: this.state.data, onChange: this.handleChange });\n        }\n    }]);\n\n    return Demo;\n}(React.Component);\n\nReactDOM.render(React.createElement(Demo, null), mountNode);})()</script><div class=\"highlight\"><pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> CascaderSelect <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">'@alifd/next'</span><span class=\"token punctuation\">;</span>\n\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">Demo</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\n    <span class=\"token function\">constructor</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">props</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">super</span><span class=\"token punctuation\">(</span>props<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state <span class=\"token operator\">=</span> <span class=\"token punctuation\">{</span>\n            data<span class=\"token operator\">:</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">]</span>\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">componentDidMount</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token function\">fetch</span><span class=\"token punctuation\">(</span><span class=\"token string\">'https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json'</span><span class=\"token punctuation\">)</span>\n            <span class=\"token punctuation\">.</span><span class=\"token function\">then</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">response</span> <span class=\"token operator\">=></span> response<span class=\"token punctuation\">.</span><span class=\"token function\">json</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span>\n            <span class=\"token punctuation\">.</span><span class=\"token function\">then</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">data</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n                <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span> data <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n            <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span>\n            <span class=\"token punctuation\">.</span><span class=\"token function\">catch</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">e</span> <span class=\"token operator\">=></span> console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>e<span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function-variable function\">handleChange</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token parameter\">value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\n        console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\n        <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">CascaderSelect</span></span> <span class=\"token attr-name\">dataSource</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state<span class=\"token punctuation\">.</span>data<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">onChange</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>handleChange<span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">;</span>\n    <span class=\"token punctuation\">}</span>\n<span class=\"token punctuation\">}</span>\n\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Demo</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span></code></pre></div>","renderScript":"<script>(function(){'use strict';\n\nvar _createClass = function () { function defineProperties(target, props) { for (var i = 0; i < props.length; i++) { var descriptor = props[i]; descriptor.enumerable = descriptor.enumerable || false; descriptor.configurable = true; if (\"value\" in descriptor) descriptor.writable = true; Object.defineProperty(target, descriptor.key, descriptor); } } return function (Constructor, protoProps, staticProps) { if (protoProps) defineProperties(Constructor.prototype, protoProps); if (staticProps) defineProperties(Constructor, staticProps); return Constructor; }; }();\n\nvar _reactLive = require('react-live');\n\nvar _next = require('@alifd/next');\n\nfunction _classCallCheck(instance, Constructor) { if (!(instance instanceof Constructor)) { throw new TypeError(\"Cannot call a class as a function\"); } }\n\nfunction _possibleConstructorReturn(self, call) { if (!self) { throw new ReferenceError(\"this hasn't been initialised - super() hasn't been called\"); } return call && (typeof call === \"object\" || typeof call === \"function\") ? call : self; }\n\nfunction _inherits(subClass, superClass) { if (typeof superClass !== \"function\" && superClass !== null) { throw new TypeError(\"Super expression must either be null or a function, not \" + typeof superClass); } subClass.prototype = Object.create(superClass && superClass.prototype, { constructor: { value: subClass, enumerable: false, writable: true, configurable: true } }); if (superClass) Object.setPrototypeOf ? Object.setPrototypeOf(subClass, superClass) : subClass.__proto__ = superClass; }\n\nwindow.demoNames.push('basicEnUs');\n\n\nwindow.basicEnUsRenderScript = function basicEnUsRenderScript(liveDemo) {\n    var mountNode = document.getElementById('basicEnUs-mount');\n    if (liveDemo === \"false\") {\n        document.getElementById('basicEnUs-body').innerHTML = '<pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> CascaderSelect <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">\\'@alifd/next\\'</span><span class=\"token punctuation\">;</span>\\n\\n<span class=\"token keyword\">class</span> <span class=\"token class-name\">Demo</span> <span class=\"token keyword\">extends</span> <span class=\"token class-name\">React<span class=\"token punctuation\">.</span>Component</span> <span class=\"token punctuation\">{</span>\\n    <span class=\"token function\">constructor</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">props</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\\n        <span class=\"token keyword\">super</span><span class=\"token punctuation\">(</span>props<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\\n\\n        <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state <span class=\"token operator\">=</span> <span class=\"token punctuation\">{</span>\\n            data<span class=\"token operator\">:</span> <span class=\"token punctuation\">[</span><span class=\"token punctuation\">]</span>\\n        <span class=\"token punctuation\">}</span><span class=\"token punctuation\">;</span>\\n    <span class=\"token punctuation\">}</span>\\n\\n    <span class=\"token function\">componentDidMount</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\\n        <span class=\"token function\">fetch</span><span class=\"token punctuation\">(</span><span class=\"token string\">\\'https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json\\'</span><span class=\"token punctuation\">)</span>\\n            <span class=\"token punctuation\">.</span><span class=\"token function\">then</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">response</span> <span class=\"token operator\">=></span> response<span class=\"token punctuation\">.</span><span class=\"token function\">json</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span>\\n            <span class=\"token punctuation\">.</span><span class=\"token function\">then</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">data</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\\n                <span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span><span class=\"token function\">setState</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">{</span> data <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\\n            <span class=\"token punctuation\">}</span><span class=\"token punctuation\">)</span>\\n            <span class=\"token punctuation\">.</span><span class=\"token function\">catch</span><span class=\"token punctuation\">(</span><span class=\"token parameter\">e</span> <span class=\"token operator\">=></span> console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>e<span class=\"token punctuation\">)</span><span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\\n    <span class=\"token punctuation\">}</span>\\n\\n    <span class=\"token function-variable function\">handleChange</span> <span class=\"token operator\">=</span> <span class=\"token punctuation\">(</span><span class=\"token parameter\">value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra</span><span class=\"token punctuation\">)</span> <span class=\"token operator\">=></span> <span class=\"token punctuation\">{</span>\\n        console<span class=\"token punctuation\">.</span><span class=\"token function\">log</span><span class=\"token punctuation\">(</span>value<span class=\"token punctuation\">,</span> data<span class=\"token punctuation\">,</span> extra<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\\n    <span class=\"token punctuation\">}</span>\\n\\n    <span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token punctuation\">)</span> <span class=\"token punctuation\">{</span>\\n        <span class=\"token keyword\">return</span> <span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">CascaderSelect</span></span> <span class=\"token attr-name\">dataSource</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>state<span class=\"token punctuation\">.</span>data<span class=\"token punctuation\">}</span></span> <span class=\"token attr-name\">onChange</span><span class=\"token script language-javascript\"><span class=\"token script-punctuation punctuation\">=</span><span class=\"token punctuation\">{</span><span class=\"token keyword\">this</span><span class=\"token punctuation\">.</span>handleChange<span class=\"token punctuation\">}</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">;</span>\\n    <span class=\"token punctuation\">}</span>\\n<span class=\"token punctuation\">}</span>\\n\\nReactDOM<span class=\"token punctuation\">.</span><span class=\"token function\">render</span><span class=\"token punctuation\">(</span><span class=\"token tag\"><span class=\"token tag\"><span class=\"token punctuation\">&lt;</span><span class=\"token class-name\">Demo</span></span> <span class=\"token punctuation\">/></span></span><span class=\"token punctuation\">,</span> mountNode<span class=\"token punctuation\">)</span><span class=\"token punctuation\">;</span>\\n</code></pre>\\n'.replace(/{backquote}/g, '`').replace(/{dollar}/g, '$');\n\n        var Demo = function (_React$Component) {\n            _inherits(Demo, _React$Component);\n\n            function Demo(props) {\n                _classCallCheck(this, Demo);\n\n                var _this = _possibleConstructorReturn(this, (Demo.__proto__ || Object.getPrototypeOf(Demo)).call(this, props));\n\n                _this.handleChange = function (value, data, extra) {\n                    console.log(value, data, extra);\n                };\n\n                _this.state = {\n                    data: []\n                };\n                return _this;\n            }\n\n            _createClass(Demo, [{\n                key: 'componentDidMount',\n                value: function componentDidMount() {\n                    var _this2 = this;\n\n                    fetch('https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json').then(function (response) {\n                        return response.json();\n                    }).then(function (data) {\n                        _this2.setState({ data: data });\n                    }).catch(function (e) {\n                        return console.log(e);\n                    });\n                }\n            }, {\n                key: 'render',\n                value: function render() {\n                    return React.createElement(_next.CascaderSelect, { dataSource: this.state.data, onChange: this.handleChange });\n                }\n            }]);\n\n            return Demo;\n        }(React.Component);\n\n        ReactDOM.render(React.createElement(Demo, null), mountNode);\n\n        return;\n    }\n\n    var basicEnUsLiveScript = 'class Demo extends React.Component {\\n  constructor(props) {\\n    super(props);\\n\\n    this.handleChange = (value, data, extra) => {\\n      console.log(value, data, extra);\\n    };\\n    this.state = {\\n      data: []\\n    };\\n  }\\n\\n  componentDidMount() {\\n    fetch(\"https://os.alipayobjects.com/rmsportal/ODDwqcDFTLAguOvWEolX.json\")\\n      .then(response => response.json())\\n      .then(data => {\\n        this.setState({ data });\\n      })\\n      .catch(e => console.log(e));\\n  }\\n\\n  render() {\\n    return (\\n      <CascaderSelect\\n        dataSource={this.state.data}\\n        onChange={this.handleChange}\\n      />\\n    );\\n  }\\n}\\n\\nReactDOM.render(<Demo />, mountNode);';\n    var emptyTheme = {\n        plain: {},\n        styles: [{\n            types: [],\n            styles: {}\n        }]\n    };\n\n    function renderAfter() {\n        ReactDOM.render(React.createElement(\n            _next.Balloon.Tooltip,\n            {\n                align: 't',\n                style: { maxWidth: 320 },\n                trigger: React.createElement('div', {\n                    dangerouslySetInnerHTML: {\n                        __html: '<pre class=\"language-jsx\"><code class=\"language-jsx\"><span class=\"token keyword\">import</span> <span class=\"token punctuation\">{</span> CascaderSelect <span class=\"token punctuation\">}</span> <span class=\"token keyword\">from</span> <span class=\"token string\">\\'@alifd/next\\'</span><span class=\"token punctuation\">;</span>\\n</code></pre>\\n'\n                    }\n                })\n            },\n            '\\u7F16\\u8F91\\u6A21\\u5F0F\\u6682\\u4E0D\\u652F\\u6301\\u4FEE\\u6539\\u4F9D\\u8D56\\u5F15\\u5165'\n        ), document.getElementById('basicEnUs-live-import'));\n    }\n\n    var LiveRenderer = function (_React$Component2) {\n        _inherits(LiveRenderer, _React$Component2);\n\n        function LiveRenderer(props) {\n            _classCallCheck(this, LiveRenderer);\n\n            var _this3 = _possibleConstructorReturn(this, (LiveRenderer.__proto__ || Object.getPrototypeOf(LiveRenderer)).call(this, props));\n\n            _this3.onBlur = function () {\n                var time = new Date().getTime();\n                window.top.postMessage({\n                    type: 'ReactLiveEdit',\n                    from: 'demo',\n                    body: { name: 'basicEnUs', component: 'CascaderSelect', time: time }\n                }, '*');\n            };\n\n            return _this3;\n        }\n\n        _createClass(LiveRenderer, [{\n            key: 'componentDidMount',\n            value: function componentDidMount() {\n                renderAfter();\n            }\n        }, {\n            key: 'render',\n            value: function render() {\n                return React.createElement(\n                    _reactLive.LiveProvider,\n                    {\n                        code: basicEnUsLiveScript,\n                        scope: { CascaderSelect: _next.CascaderSelect, mountNode: mountNode },\n                        noInline: true },\n                    React.createElement(\n                        'div',\n                        { id: 'basicEnUs-live-editor' },\n                        React.createElement(_reactLive.LiveError, { id: 'basicEnUs-live-error', className: 'react-live-error' }),\n                        React.createElement('div', { id: 'basicEnUs-live-import' }),\n                        React.createElement(\n                            'div',\n                            { id: 'basicEnUs-live-body', className: 'react-live-body' },\n                            React.createElement(_reactLive.LiveEditor, { theme: emptyTheme, onBlur: this.onBlur })\n                        ),\n                        React.createElement('div', { id: 'basicEnUs-live-css' })\n                    ),\n                    React.createElement(_reactLive.LivePreview, null)\n                );\n            }\n        }]);\n\n        return LiveRenderer;\n    }(React.Component);\n\n    ReactDOM.render(React.createElement(LiveRenderer, null), document.getElementById('basicEnUs-body'));\n    return;\n};\n\nwindow.renderFuncs.push(basicEnUsRenderScript);\n\nfunction onRiddleOrCodePenClick(type) {\n    var time = new Date().getTime();\n    window.top.postMessage({\n        type: 'RiddleOrCodePenClick',\n        from: 'demo',\n        body: { name: 'basicEnUs', component: 'CascaderSelect', type: type, time: time }\n    }, '*');\n}\nReactDOM.render(React.createElement(\n    _next.Balloon.Tooltip,\n    {\n        align: 'b',\n        style: { maxWidth: 400 },\n        trigger: React.createElement(\n            'span',\n            { role: 'img', className: 'op-icon', onClick: function onClick() {\n                    return onRiddleOrCodePenClick('CodePen');\n                } },\n            React.createElement(\n                'svg',\n                { viewBox: '0 0 20 20', fill: 'currentColor' },\n                React.createElement('path', {\n                    d: 'M17.7207447,7.0537234 L10.2739362,2.0893617 C10.0952128,1.97021277 9.86223404,1.97021277 9.68404255,2.0893617 L2.23723404,7.0537234 C2.0893617,7.15212766 2.00053191,7.31861702 2.00053191,7.4962766 L2.00053191,12.4606383 C2.00053191,12.6382979 2.0893617,12.8047872 2.23723404,12.9031915 L9.68404255,17.8675532 C9.77340426,17.9271277 9.87606383,17.9569149 9.97925532,17.9569149 C10.0824468,17.9569149 10.1851064,17.9271277 10.2744681,17.8675532 L17.7212766,12.9031915 C17.8691489,12.8047872 17.9579787,12.6382979 17.9579787,12.4606383 L17.9579787,7.4962766 C17.9579787,7.31861702 17.8691489,7.15212766 17.7212766,7.0537234 L17.7207447,7.0537234 Z M9.9787234,11.8218085 L7.2143617,9.9787234 L9.9787234,8.1356383 L12.7430851,9.9787234 L9.9787234,11.8218085 Z M10.5106383,7.21170213 L10.5106383,3.52553191 L16.4664894,7.4962766 L13.7021277,9.3393617 L10.5106383,7.21170213 Z M9.44680851,7.21170213 L6.25531915,9.3393617 L3.49095745,7.4962766 L9.44680851,3.52553191 L9.44680851,7.21170213 Z M5.2962766,9.9787234 L3.06382979,11.4670213 L3.06382979,8.49042553 L5.2962766,9.9787234 Z M6.25531915,10.6180851 L9.44680851,12.7457447 L9.44680851,16.4319149 L3.49095745,12.4611702 L6.25531915,10.6180851 Z M10.5106383,12.7457447 L13.7021277,10.6180851 L16.4664894,12.4611702 L10.5106383,16.4319149 L10.5106383,12.7457447 Z M14.6611702,9.9787234 L16.893617,8.49042553 L16.893617,11.4670213 L14.6611702,9.9787234 Z' })\n            )\n        ) },\n    React.createElement(\n        'span',\n        null,\n        '\\u5728CodePen\\u4E2D\\u6253\\u5F00'\n    )\n), document.getElementById('basicEnUs-CodePen'));\nReactDOM.render(React.createElement(\n    _next.Balloon.Tooltip,\n    {\n        align: 'b',\n        style: { maxWidth: 400 },\n        trigger: React.createElement(\n            'span',\n            { role: 'img', className: 'op-icon', onClick: function onClick() {\n                    return onRiddleOrCodePenClick('Riddle');\n                } },\n            React.createElement(\n                'svg',\n                { viewBox: '0 0 20 20', fill: 'currentColor' },\n                React.createElement('path', {\n                    d: 'M12.0135981,2 C14.9585189,2 17.345849,4.38716704 17.345849,7.33333333 C17.345849,9.38478693 16.1882418,11.1657179 14.4903288,12.0578577 L17.2084049,16.7658872 C17.2378708,16.8169235 17.2591949,16.8704263 17.2727803,16.9248914 C17.3474476,17.0262914 17.3916465,17.1520943 17.3916465,17.2882205 C17.3916465,17.628088 17.1161295,17.9036051 16.7762619,17.9036051 L2.81174505,17.9048498 C2.75007855,17.9255976 2.68404472,17.9368421 2.61538462,17.9368421 C2.27551708,17.9368421 2,17.661325 2,17.3214575 L2,4.90050552 C2,4.44767651 2.36696407,4.08058607 2.8201909,4.08058607 L2.8201909,4.08058607 L4.598,4.08 L4.59829061,3.64037695 C4.59829061,2.78210363 5.25867561,2.07778272 6.09736436,2.00602116 L6.23871411,2 Z M11.9839597,3.23076923 L6.23745245,3.23076923 C6.01143198,3.23076923 5.82905984,3.41419855 5.82905984,3.64047008 L5.82905984,3.64047008 L5.829,4.08 L11.5615101,4.08058607 C13.3089935,4.08058607 14.7370181,5.4476011 14.8334247,7.17082808 L14.8386124,7.35677655 C14.8386124,9.16616658 13.3721154,10.632967 11.5615101,10.632967 L11.5615101,10.632967 L10.299,10.632 L12.6155561,14.6429723 C12.7020335,14.7927556 12.7183875,14.9637818 12.6748043,15.1180362 C12.6779184,15.1342067 12.6786336,15.1513556 12.6786336,15.1686715 C12.6786336,15.508539 12.4031165,15.7840561 12.063249,15.7840561 L5.39477011,15.7840561 C5.33908357,15.7840561 5.28512459,15.7766596 5.23382202,15.7627953 L5.21367522,15.7639098 L5.21367522,15.7639098 C4.87380768,15.7639098 4.59829061,15.4883927 4.59829061,15.1485252 L4.598,5.323 L3.23076923,5.32307709 L3.23,16.672 L15.733,16.672 L13.0769083,12.0713449 C12.9069827,11.7770252 13.0078241,11.40068 13.3021438,11.2307544 C13.3538063,11.200927 13.4079962,11.1794424 13.4631533,11.1658825 C14.9972153,10.5673738 16.0854701,9.07745387 16.0854701,7.33333333 C16.0854701,5.06705157 14.2491614,3.23076923 11.9839597,3.23076923 L11.9839597,3.23076923 Z M11.7212434,5.32867389 L11.5688942,5.32307709 L5.829,5.323 L5.82905984,11.0261966 C5.82905984,11.0464748 5.83052125,11.0664018 5.83334393,11.0858783 L5.84579569,11.1428571 L5.829,11.142 L5.829,14.553 L11.142,14.553 L8.71393544,10.3467056 C8.54400168,10.0523717 8.64484792,9.67600839 8.93918185,9.50607462 C9.01663814,9.46135521 9.09977514,9.43538787 9.18333591,9.42676402 L9.18350929,9.40512829 L11.5688942,9.40512829 C12.6982428,9.40512829 13.6102561,8.49132999 13.6102561,7.36410269 C13.6102561,6.23662753 12.6963072,5.32307709 11.5688942,5.32307709 Z' })\n            )\n        ) },\n    React.createElement(\n        'span',\n        null,\n        '\\u5728Riddle\\u4E2D\\u6253\\u5F00'\n    )\n), document.getElementById('basicEnUs-Riddle'));\nReactDOM.render(React.createElement(\n    _next.Balloon.Tooltip,\n    {\n        align: 'b',\n        style: { maxWidth: 320 },\n        trigger: React.createElement(\n            'span',\n            { className: 'code-box-code-action', onClick: function onClick() {\n                    _next.Message.success('复制成功');\n                } },\n            React.createElement(\n                'svg',\n                { viewBox: '0 0 20 20', focusable: 'false', 'data-icon': 'snippets', width: '20px', height: '20px', fill: 'currentColor', 'aria-hidden': 'true' },\n                React.createElement('path', { d: 'M15,5 L15,18 L2,18 L2,5 L15,5 Z M14,6 L3,6 L3,17 L14,17 L14,6 Z M18,2 L18,15 L16,15 L16,13.999 L17,14 L17,3 L6,3 L6,4 L5,4 L5,2 L18,2 Z M9,8 L9,11 L12,11 L12,12 L9,12 L9,15 L8,15 L8,12 L5,12 L5,11 L8,11 L8,8 L9,8 Z' })\n            )\n        )\n    },\n    React.createElement(\n        'span',\n        null,\n        '\\u590D\\u5236\\u4EE3\\u7801'\n    )\n), document.getElementById('basicEnUs-copy-btn'));\nReactDOM.render(React.createElement(\n    React.Fragment,\n    null,\n    React.createElement(\n        _next.Balloon.Tooltip,\n        {\n            align: 'b',\n            style: { maxWidth: 400 },\n            trigger: React.createElement(\n                'span',\n                { id: 'basicEnUs-icon-show', className: 'code-box-code-action code-expand-icon-show' },\n                React.createElement(\n                    'svg',\n                    { alt: 'expand code', width: '20px', height: '20px', viewBox: '0 0 20 20', fill: 'currentColor' },\n                    React.createElement('path', {\n                        d: 'M14.4307124,13.5667899 L15.1349452,14.276759 L10.7473676,18.6288871 L6.42783259,14.2738791 L7.13782502,13.5696698 L10.7530744,17.2147744 L14.4307124,13.5667899 Z M4.79130753,8.067524 L16.3824174,11.1733525 L16.1235984,12.1392784 L4.53248848,9.03344983 L4.79130753,8.067524 Z M10.8154102,1.57503552 L15.1349452,5.93004351 L14.4249528,6.63425282 L10.809949,2.98914817 L7.13206544,6.6371327 L6.42783259,5.92716363 L10.8154102,1.57503552 Z',\n                        transform: 'translate(10.457453, 10.101961) rotate(90.000000) translate(-10.457453, -10.101961) ' })\n                )\n            ) },\n        React.createElement(\n            'span',\n            null,\n            '\\u5C55\\u5F00\\u4EE3\\u7801',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            '\\u5C0F\\u63D0\\u793A: ',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            ' 1. \\u70B9\\u51FB\\u4E00\\u4E0B\\u4EE3\\u7801\\uFF0C\\u8BD5\\u4E00\\u8BD5\\u5728\\u7EBF\\u7F16\\u8F91\\u9884\\u89C8\\u5427\\uFF01 ',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            '2. \\u9875\\u9762\\u53F3\\u4E0A\\u65B9 \\u6709 ',\n            React.createElement(\n                'strong',\n                null,\n                '\\u5168\\u5C40\\u4EE3\\u7801\\u5C55\\u5F00'\n            ),\n            ' \\u53CA ',\n            React.createElement(\n                'strong',\n                null,\n                '\\u5F00\\u542F\\u5728\\u7EBF\\u7F16\\u8F91'\n            ),\n            ' \\u6A21\\u5F0F\\u54DF\\uFF5E'\n        )\n    ),\n    React.createElement(\n        _next.Balloon.Tooltip,\n        {\n            align: 'b',\n            style: { maxWidth: 400 },\n            trigger: React.createElement(\n                'span',\n                { id: 'basicEnUs-icon-hide', className: 'code-box-code-action code-expand-icon-hide', style: { display: 'none' } },\n                React.createElement(\n                    'svg',\n                    { alt: 'expand code', width: '20px', height: '20px', viewBox: '0 0 20 20', style: { fill: '#3B9AFF' } },\n                    React.createElement('path', {\n                        d: 'M14.4307124,13.5667899 L15.1349452,14.276759 L10.7473676,18.6288871 L6.42783259,14.2738791 L7.13782502,13.5696698 L10.7530744,17.2147744 L14.4307124,13.5667899 Z M4.79130753,8.067524 L16.3824174,11.1733525 L16.1235984,12.1392784 L4.53248848,9.03344983 L4.79130753,8.067524 Z M10.8154102,1.57503552 L15.1349452,5.93004351 L14.4249528,6.63425282 L10.809949,2.98914817 L7.13206544,6.6371327 L6.42783259,5.92716363 L10.8154102,1.57503552 Z',\n                        transform: 'translate(10.457453, 10.101961) rotate(90.000000) translate(-10.457453, -10.101961) ' })\n                )\n            ) },\n        React.createElement(\n            'span',\n            null,\n            '\\u6536\\u8D77\\u4EE3\\u7801',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            '\\u5C0F\\u63D0\\u793A: ',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            ' 1. \\u70B9\\u51FB\\u4E00\\u4E0B\\u4EE3\\u7801\\uFF0C\\u8BD5\\u4E00\\u8BD5\\u5728\\u7EBF\\u7F16\\u8F91\\u9884\\u89C8\\u5427\\uFF01 ',\n            React.createElement('br', null),\n            React.createElement('br', null),\n            '2. \\u9875\\u9762\\u53F3\\u4E0A\\u65B9 \\u6709 ',\n            React.createElement(\n                'strong',\n                null,\n                '\\u5168\\u5C40\\u4EE3\\u7801\\u5C55\\u5F00'\n            ),\n            ' \\u53CA ',\n            React.createElement(\n                'strong',\n                null,\n                '\\u5F00\\u542F\\u5728\\u7EBF\\u7F16\\u8F91'\n            ),\n            ' \\u6A21\\u5F0F\\u54DF\\uFF5E'\n        )\n    )\n), document.getElementById('basicEnUs-fold-code'));})()</script>"}
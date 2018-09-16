
[原始 README](#original)

# 说明

[browser-amd-editor](/browser-amd-editor)  编辑器

[browser-amd-diff-editor](/browser-amd-diff-editor)  显示差异

[browser-amd-iframe](/browser-amd-iframe) iframe

延迟3秒显示 4 个 iframe , 前3个由 css 控制了 大小/可见性 ,所以一开始不可见 , 第四个是由 js 动态创建

	0x0 width: {width: 0; height: 0;}  --> {width: 400px; height: 100px; display:'block' ;visibility:'visible'}
	display:none: {display: none;}  --> {width: 400px; height: 100px; display:'block' ;visibility:'visible'}
	visibility:hidden: {visibility: hidden;}  --> {width: 400px; height: 100px; display:'block' ;visibility:'visible'}
	taken off-dom while loading: {}  --> {width: 400px; height: 100px; display:'block' ;visibility:'visible'}


[browser-amd-localized](/browser-amd-localized) 本地化 德语

[browser-amd-monarch](/browser-amd-monarch) monarch 语法高亮

日志 语法 高亮 `error` `info` `notice` `date` 等信息

	tokenizer: {
					root: [
						[/\[error.*/, "custom-error"],
						[/\[notice.*/, "custom-notice"],
						[/\[info.*/, "custom-info"],
						[/\[[a-zA-Z 0-9:]+\]/, "custom-date"],
					],
				}

[browser-amd-requirejs](/browser-amd-requirejs) Loading with requirejs


[browser-amd-shared-model](/browser-amd-shared-model) 共享模型

 两个编辑器同步修改代码

[browser-script-editor](/browser-script-editor) Sync Loading Sample 同步加载

[browser-undo-redo-controls](/browser-undo-redo-controls) 撤销 重做控制

[browser-esm-parcel](/browser-esm-parcel)
[browser-esm-webpack](/browser-esm-webpack)
[browser-esm-webpack-small](/browser-esm-webpack-small)


[electron-amd](/electron-amd)
[node_modules](/node_modules)
[nwjs-amd](/nwjs-amd)
[nwjs-amd-v2](/nwjs-amd-v2)




# original

# Monaco Editor Samples

Standalone HTML samples showing how to integrate the Monaco Editor.

## Running

```
git clone https://github.com/Microsoft/monaco-editor-samples.git
cd monaco-editor-samples
npm install .
npm run simpleserver
```

Go to <a href="http://localhost:8888">localhost:8888</a> and explore the samples!

## Loading variations
* `browser-amd-editor`: running in a browser using `AMD` lazy loading.
* `browser-script-editor`: running in a browser using `AMD` synchronous loading via `<script>` tags.
* `browser-esm-webpack`: running in a browser using webpack.
* `browser-esm-webpack-small`: running in a browser using webpack (only a subset of the editor).
* `electron-amd`: running in electron.
* `nwjs-amd` and `nwjs-amd-v2`: running in nwjs. it is reported that v2 works and the initial version does not.

## Other examples & techniques
* `browser-amd-diff-editor`: running the diff editor in a browser.
* `browser-amd-iframe`: running in an `<iframe>`.
* `browser-amd-localized`: running with the `German` locale.
* `browser-amd-monarch`: running with a custom language grammar written with Monarch.
* `browser-amd-shared-model`: using the same text model in two editors.

## License

MIT

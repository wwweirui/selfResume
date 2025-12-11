<script setup lang="ts">
const publicConfig = useRuntimeConfig().public

const name = publicConfig.name 
const phone = publicConfig.phone

useSeoMeta({
	title: `${name} - 前端开发`,
	description: `${name}前端开发简历`,
	robots: 'noindex, nofollow',
})
</script>

<template>
<Builder class="block print:hidden" w="fit" m="is-auto x-1 y-.5" />
<article
	bg="white @dark:slate/10 print:transparent"
	p="6 print:x-2 print:y-0"
	text="3.7"
	tracking="wide"
	rounded="xl print:0"
>
	<h1 text="center" m="be-4">
		{{ `${name}-前端工程师` }}
	</h1>

	<ul columns="sm:1" p="is-0">
		<!-- <InfoLi icon="ri:smartphone-line" label="电话">
			{{ phone }} (同微信)
		</InfoLi> -->
		<InfoLi icon="gravity-ui:person" label="">
			叶伟睿 / 男 / 28岁 / 上海
		</InfoLi>
				
		<InfoLi icon="icon-park-outline:phone" label="">
			136-8708-3589
		</InfoLi>

		<InfoLi icon="ri:mail-line" label="邮箱">
			<InfoLink to="mailto:weiruiye@foxmail.com" />
		</InfoLi>
		

		<!-- <InfoLi icon="ri:github-line" label="GitHub">
			<InfoLink to="https://github.com/wwweirui">
				wwweirui
			</InfoLink>
		</InfoLi> -->


		<!-- <InfoLi icon="ri:school-line" label="学校">
			辽宁大学 (软件工程)
		</InfoLi> -->

		<!-- <InfoLi icon="ri:graduation-cap-line" label="学历">
			本科在读 (2026 届)
		</InfoLi> -->
	</ul>

	<InfoSection title="教育背景">
		<ul>
			<li>硕士研究生-辽宁大学-软件工程专硕 （2019 - 2022）</li>
			<li>本科-华东交通大学-软件工程+交通运输（2015 - 2019）</li>
		</ul>
	</InfoSection>

	<InfoSection title="专业技能">
		<ul>
			<li>熟悉前端基础 HTML CSS ES6+ JS TS 语法，熟悉 HTTP 协议</li>
			<li>掌握 Vue 3、Nuxt 4、TypeScript，熟练掌握响应式设计、UI/UX 优化</li>
			<li>善于运用 AI 工具提升开发效能，注重代码质量与兼容性实践</li>
			<li>软件设计师（中级）</li>
			<li>证券从业资格证，基金从业资格证</li>
		</ul>
	</InfoSection>

	<InfoSection title="工作经历">
		<Project
			name="德邦证券股份有限公司"
			desc="投研科技组-前端开发"
			from="2022.07"
		>
			<ul>
				<li>负责并参与公司B端业务需求支持，设计技术方案，完成多版本迭代</li>
				<li>独立完成H5项目搭建，完成项目上线</li>
				<li>维护团队组件库，搭建文档，针对业务场景二次封装开发</li>
				<li>知识库产出，参与团队前端规范构建，周例会知识分享</li>
			</ul>
		</Project>
	</InfoSection>

	<InfoSection title="项目经验">
		<!-- <Project
			name="blog-v3"
			desc="个人博客"
			role="创建者"
			link="https://github.com/L33Z22L11/blog-v3"
			from="2024.08"
			:techs="['Nuxt', 'Vue 3', 'TypeScript', 'Pinia', 'Scss']"
		>
			<ul>
				<li>开源项目获 120+Stars，15+真实下游用户，通过 GitHub、交流群持续迭代项目，适配多个云构建平台的 SSR/SSG 功能。</li>
				<li>发现上游多处不合预期的问题，通过提交 Issue / PR、打 Patch 等方式修复。</li>
				<li>精校响应式设计、深色模式体验、文字排版布局，设计风格优雅统一，组件系统完善。</li>
				<li>通过 Google Search Console 监测发现境外繁体镜像站点，参阅 Whois、HTTP Header 等信息，定位到 Cloudflare 反代 + 域名替换的行为机制，开发出恶意反代跳转回原站的方案；同时排查 SEO 问题，优化至月 PV 10K。</li>
			</ul>
		</Project>

		<Project
			name="GioPic"
			desc="图床上传桌面程序"
			role="核心贡献者"
			link="https://github.com/isYangs/GioPic"
			from="2024.08"
			to="2025.02"
			:techs="['Electron', 'Vue 3', 'TypeScript', 'Axios', 'UnoCSS', 'NaiveUI']"
		>
			<ul>
				<li>解决跨平台启动问题，在 macOS 开发的项目在 Windows 上无法启动，通过查阅报错资料，修改构建脚本，实现多平台开发运行。</li>
				<li>提升项目扩展性，针对适配 AWS S3 / 第三方 OSS 存储源时代码扩展性差的问题，重构图床存储程序定义代码，实现第三方图床存储兼容。</li>
				<li>优化图标显示，针对 Windows 托盘图标、macOS 启动台图标比例异常问题，参考 Electron、Apple Developer 等文档规范，使用原型设计工具绘制图标并调整逻辑，实现多系统、多颜色模式下托盘、桌面图标完美显示。</li>
			</ul>
		</Project> -->
	</InfoSection>

</article>
</template>

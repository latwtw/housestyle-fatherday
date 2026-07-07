<html lang="zh-TW"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>測出最適合你的浴室設計：找尋專屬你的衛浴美學風格｜HouseStyle 好時代衛浴</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Google Fonts: Inter & Noto Sans TC -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&amp;family=Noto+Sans+TC:wght@300;400;500;700&amp;display=swap" rel="stylesheet">
    <!-- FontAwesome for Premium Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Three.js for 3D simulation -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        brandBlue: {
                            50: '#f0f7ff',
                            100: '#e0effe',
                            200: '#bae0fd',
                            300: '#7cc7fb',
                            400: '#38abf8',
                            500: '#0e90e9',
                            600: '#0072c6', /* HouseStyle brand primary */
                            700: '#025ba2',
                            800: '#064e86',
                            900: '#0b416f',
                            950: '#07294a'
                        },
                        neutralWhite: '#fcfdfe',
                        premiumGray: '#f1f5f9'
                    },
                    fontFamily: {
                        sans: ['Inter', 'Noto Sans TC', 'sans-serif'],
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Inter', 'Noto Sans TC', sans-serif;
            overflow-x: hidden;
            background-color: #f0f7ff;
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 6px;
        }
        ::-webkit-scrollbar-track {
            background: #f0f7ff;
        }
        ::-webkit-scrollbar-thumb {
            background: #bae0fd;
            border-radius: 3px;
        }
        /* Glassmorphism utility */
        .glass-panel {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(16px);
            -webkit-backdrop-filter: blur(16px);
            border: 1px solid rgba(255, 255, 255, 0.6);
            box-shadow: 0 10px 30px rgba(0, 114, 198, 0.08);
        }
        .btn-glow {
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        .btn-glow:hover {
            box-shadow: 0 0 20px rgba(0, 114, 198, 0.4);
            transform: translateY(-2px);
        }
        /* Page animation states */
        .show-page {
            opacity: 1;
            transform: scale(1);
            transition: all 0.6s cubic-bezier(0.16, 1, 0.3, 1);
            pointer-events: auto;
            position: relative;
            z-index: 10;
        }
        .hide-page {
            opacity: 0;
            transform: scale(0.95);
            pointer-events: none;
            position: absolute;
            width: 100%;
            z-index: 0;
            display: none !important;
        }
        /* 3D Canvas Background fixed full */
        #webgl-container {
            position: fixed;
            top: 0;
            left: 0;
            width: 100vw;
            height: 100vh;
            z-index: 1;
            pointer-events: none;
        }
    </style>
<style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:Inter, Noto Sans TC, sans-serif;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.pointer-events-none{pointer-events:none}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.inset-0{inset:0px}.left-1\/2{left:50%}.top-8{top:2rem}.z-10{z-index:10}.z-20{z-index:20}.z-50{z-index:50}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-2{margin-bottom:0.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mt-4{margin-top:1rem}.mr-2{margin-right:0.5rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.grid{display:grid}.aspect-\[4\/3\]{aspect-ratio:4/3}.h-1\.5{height:0.375rem}.h-16{height:4rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-1\/5{width:20%}.w-16{width:4rem}.w-8{width:2rem}.w-full{width:100%}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1\/2{--tw-translate-x:-50%;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-0{--tw-translate-y:0px;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;user-select:none}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-3{gap:0.75rem}.gap-8{gap:2rem}.space-x-1\.5 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.375rem * var(--tw-space-x-reverse));margin-left:calc(0.375rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-3 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.75rem * var(--tw-space-x-reverse));margin-left:calc(0.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(0.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(0.25rem * var(--tw-space-y-reverse))}.space-y-4 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-t{border-top-width:1px}.border-brandBlue-100{--tw-border-opacity:1;border-color:rgb(224 239 254 / var(--tw-border-opacity, 1))}.border-brandBlue-200{--tw-border-opacity:1;border-color:rgb(186 224 253 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225 / var(--tw-border-opacity, 1))}.border-white\/20{border-color:rgb(255 255 255 / 0.2)}.border-white\/80{border-color:rgb(255 255 255 / 0.8)}.bg-\[\#06C755\]{--tw-bg-opacity:1;background-color:rgb(6 199 85 / var(--tw-bg-opacity, 1))}.bg-brandBlue-100{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.bg-brandBlue-50{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.bg-brandBlue-600{--tw-bg-opacity:1;background-color:rgb(0 114 198 / var(--tw-bg-opacity, 1))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-white\/10{background-color:rgb(255 255 255 / 0.1)}.bg-white\/40{background-color:rgb(255 255 255 / 0.4)}.bg-white\/60{background-color:rgb(255 255 255 / 0.6)}.bg-white\/70{background-color:rgb(255 255 255 / 0.7)}.bg-gradient-to-r{background-image:linear-gradient(to right, var(--tw-gradient-stops))}.bg-gradient-to-t{background-image:linear-gradient(to top, var(--tw-gradient-stops))}.from-brandBlue-600{--tw-gradient-from:#0072c6 var(--tw-gradient-from-position);--tw-gradient-to:rgb(0 114 198 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.from-slate-900\/40{--tw-gradient-from:rgb(15 23 42 / 0.4) var(--tw-gradient-from-position);--tw-gradient-to:rgb(15 23 42 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.to-brandBlue-800{--tw-gradient-to:#064e86 var(--tw-gradient-to-position)}.to-transparent{--tw-gradient-to:transparent var(--tw-gradient-to-position)}.object-cover{object-fit:cover}.p-3{padding:0.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-10{padding-left:2.5rem;padding-right:2.5rem}.px-3{padding-left:0.75rem;padding-right:0.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-1\.5{padding-top:0.375rem;padding-bottom:0.375rem}.py-2\.5{padding-top:0.625rem;padding-bottom:0.625rem}.py-3\.5{padding-top:0.875rem;padding-bottom:0.875rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-8{padding-top:2rem;padding-bottom:2rem}.pl-2{padding-left:0.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-\[9px\]{font-size:9px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.font-black{font-weight:900}.font-bold{font-weight:700}.font-extrabold{font-weight:800}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-snug{line-height:1.375}.leading-tight{line-height:1.25}.tracking-wide{letter-spacing:0.025em}.tracking-wider{letter-spacing:0.05em}.tracking-widest{letter-spacing:0.1em}.text-brandBlue-200{--tw-text-opacity:1;color:rgb(186 224 253 / var(--tw-text-opacity, 1))}.text-brandBlue-50{--tw-text-opacity:1;color:rgb(240 247 255 / var(--tw-text-opacity, 1))}.text-brandBlue-600{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.text-brandBlue-700{--tw-text-opacity:1;color:rgb(2 91 162 / var(--tw-text-opacity, 1))}.text-green-100{--tw-text-opacity:1;color:rgb(220 252 231 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-slate-950{--tw-text-opacity:1;color:rgb(2 6 23 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-yellow-300{--tw-text-opacity:1;color:rgb(253 224 71 / var(--tw-text-opacity, 1))}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-md{--tw-shadow:0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-xl{--tw-shadow:0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.backdrop-blur-md{--tw-backdrop-blur:blur(12px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.duration-200{transition-duration:200ms}.duration-300{transition-duration:300ms}.duration-500{transition-duration:500ms}.hover\:scale-\[1\.02\]:hover{--tw-scale-x:1.02;--tw-scale-y:1.02;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:border-brandBlue-400:hover{--tw-border-opacity:1;border-color:rgb(56 171 248 / var(--tw-border-opacity, 1))}.hover\:bg-\[\#05b04b\]:hover{--tw-bg-opacity:1;background-color:rgb(5 176 75 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-100:hover{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-50:hover{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-700:hover{--tw-bg-opacity:1;background-color:rgb(2 91 162 / var(--tw-bg-opacity, 1))}.group:hover .group-hover\:scale-105{--tw-scale-x:1.05;--tw-scale-y:1.05;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@media (min-width: 640px){.sm\:w-auto{width:auto}.sm\:grid-cols-3{grid-template-columns:repeat(3, minmax(0, 1fr))}}@media (min-width: 768px){.md\:col-span-5{grid-column:span 5 / span 5}.md\:col-span-7{grid-column:span 7 / span 7}.md\:aspect-square{aspect-ratio:1 / 1}.md\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}.md\:p-10{padding:2.5rem}.md\:p-12{padding:3rem}.md\:px-12{padding-left:3rem;padding-right:3rem}.md\:py-12{padding-top:3rem;padding-bottom:3rem}.md\:text-2xl{font-size:1.5rem;line-height:2rem}.md\:text-3xl{font-size:1.875rem;line-height:2.25rem}.md\:text-4xl{font-size:2.25rem;line-height:2.5rem}.md\:text-lg{font-size:1.125rem;line-height:1.75rem}.md\:text-sm{font-size:0.875rem;line-height:1.25rem}}</style><style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:Inter, Noto Sans TC, sans-serif;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.pointer-events-none{pointer-events:none}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.inset-0{inset:0px}.left-1\/2{left:50%}.top-8{top:2rem}.z-10{z-index:10}.z-20{z-index:20}.z-50{z-index:50}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-2{margin-bottom:0.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mr-1{margin-right:0.25rem}.mr-2{margin-right:0.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.grid{display:grid}.aspect-\[4\/3\]{aspect-ratio:4/3}.h-1\.5{height:0.375rem}.h-16{height:4rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-1\/5{width:20%}.w-16{width:4rem}.w-8{width:2rem}.w-full{width:100%}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1\/2{--tw-translate-x:-50%;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-0{--tw-translate-y:0px;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;user-select:none}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-3{gap:0.75rem}.gap-8{gap:2rem}.space-x-1\.5 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.375rem * var(--tw-space-x-reverse));margin-left:calc(0.375rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-3 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.75rem * var(--tw-space-x-reverse));margin-left:calc(0.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(0.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(0.25rem * var(--tw-space-y-reverse))}.space-y-4 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-t{border-top-width:1px}.border-brandBlue-100{--tw-border-opacity:1;border-color:rgb(224 239 254 / var(--tw-border-opacity, 1))}.border-brandBlue-200{--tw-border-opacity:1;border-color:rgb(186 224 253 / var(--tw-border-opacity, 1))}.border-slate-100{--tw-border-opacity:1;border-color:rgb(241 245 249 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225 / var(--tw-border-opacity, 1))}.border-white\/20{border-color:rgb(255 255 255 / 0.2)}.border-white\/80{border-color:rgb(255 255 255 / 0.8)}.bg-\[\#06C755\]{--tw-bg-opacity:1;background-color:rgb(6 199 85 / var(--tw-bg-opacity, 1))}.bg-brandBlue-100{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.bg-brandBlue-50{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.bg-brandBlue-600{--tw-bg-opacity:1;background-color:rgb(0 114 198 / var(--tw-bg-opacity, 1))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-white\/10{background-color:rgb(255 255 255 / 0.1)}.bg-white\/40{background-color:rgb(255 255 255 / 0.4)}.bg-white\/60{background-color:rgb(255 255 255 / 0.6)}.bg-white\/70{background-color:rgb(255 255 255 / 0.7)}.bg-gradient-to-r{background-image:linear-gradient(to right, var(--tw-gradient-stops))}.bg-gradient-to-t{background-image:linear-gradient(to top, var(--tw-gradient-stops))}.from-brandBlue-600{--tw-gradient-from:#0072c6 var(--tw-gradient-from-position);--tw-gradient-to:rgb(0 114 198 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.from-slate-900\/40{--tw-gradient-from:rgb(15 23 42 / 0.4) var(--tw-gradient-from-position);--tw-gradient-to:rgb(15 23 42 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.to-brandBlue-800{--tw-gradient-to:#064e86 var(--tw-gradient-to-position)}.to-transparent{--tw-gradient-to:transparent var(--tw-gradient-to-position)}.object-cover{object-fit:cover}.p-3{padding:0.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-10{padding-left:2.5rem;padding-right:2.5rem}.px-3{padding-left:0.75rem;padding-right:0.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-1\.5{padding-top:0.375rem;padding-bottom:0.375rem}.py-2\.5{padding-top:0.625rem;padding-bottom:0.625rem}.py-3\.5{padding-top:0.875rem;padding-bottom:0.875rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-8{padding-top:2rem;padding-bottom:2rem}.pl-2{padding-left:0.5rem}.pt-6{padding-top:1.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-\[9px\]{font-size:9px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.font-black{font-weight:900}.font-bold{font-weight:700}.font-extrabold{font-weight:800}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-snug{line-height:1.375}.leading-tight{line-height:1.25}.tracking-wide{letter-spacing:0.025em}.tracking-wider{letter-spacing:0.05em}.tracking-widest{letter-spacing:0.1em}.text-brandBlue-200{--tw-text-opacity:1;color:rgb(186 224 253 / var(--tw-text-opacity, 1))}.text-brandBlue-50{--tw-text-opacity:1;color:rgb(240 247 255 / var(--tw-text-opacity, 1))}.text-brandBlue-600{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.text-brandBlue-700{--tw-text-opacity:1;color:rgb(2 91 162 / var(--tw-text-opacity, 1))}.text-green-100{--tw-text-opacity:1;color:rgb(220 252 231 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-slate-950{--tw-text-opacity:1;color:rgb(2 6 23 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-yellow-300{--tw-text-opacity:1;color:rgb(253 224 71 / var(--tw-text-opacity, 1))}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-md{--tw-shadow:0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-xl{--tw-shadow:0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.backdrop-blur-md{--tw-backdrop-blur:blur(12px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.duration-200{transition-duration:200ms}.duration-300{transition-duration:300ms}.duration-500{transition-duration:500ms}.hover\:scale-\[1\.02\]:hover{--tw-scale-x:1.02;--tw-scale-y:1.02;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:border-brandBlue-400:hover{--tw-border-opacity:1;border-color:rgb(56 171 248 / var(--tw-border-opacity, 1))}.hover\:bg-\[\#05b04b\]:hover{--tw-bg-opacity:1;background-color:rgb(5 176 75 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-100:hover{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-50:hover{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-700:hover{--tw-bg-opacity:1;background-color:rgb(2 91 162 / var(--tw-bg-opacity, 1))}.hover\:text-brandBlue-600:hover{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.group:hover .group-hover\:scale-105{--tw-scale-x:1.05;--tw-scale-y:1.05;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@media (min-width: 640px){.sm\:w-auto{width:auto}.sm\:grid-cols-3{grid-template-columns:repeat(3, minmax(0, 1fr))}}@media (min-width: 768px){.md\:col-span-5{grid-column:span 5 / span 5}.md\:col-span-7{grid-column:span 7 / span 7}.md\:aspect-square{aspect-ratio:1 / 1}.md\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}.md\:p-10{padding:2.5rem}.md\:p-12{padding:3rem}.md\:px-12{padding-left:3rem;padding-right:3rem}.md\:py-12{padding-top:3rem;padding-bottom:3rem}.md\:text-2xl{font-size:1.5rem;line-height:2rem}.md\:text-3xl{font-size:1.875rem;line-height:2.25rem}.md\:text-4xl{font-size:2.25rem;line-height:2.5rem}.md\:text-lg{font-size:1.125rem;line-height:1.75rem}.md\:text-sm{font-size:0.875rem;line-height:1.25rem}}</style><style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:Inter, Noto Sans TC, sans-serif;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.pointer-events-none{pointer-events:none}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.inset-0{inset:0px}.left-1\/2{left:50%}.top-8{top:2rem}.z-10{z-index:10}.z-20{z-index:20}.z-50{z-index:50}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-2{margin-bottom:0.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mr-1{margin-right:0.25rem}.mr-2{margin-right:0.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.grid{display:grid}.aspect-\[4\/3\]{aspect-ratio:4/3}.h-1\.5{height:0.375rem}.h-16{height:4rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-1\/5{width:20%}.w-16{width:4rem}.w-8{width:2rem}.w-full{width:100%}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1\/2{--tw-translate-x:-50%;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-0{--tw-translate-y:0px;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;user-select:none}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-3{gap:0.75rem}.gap-8{gap:2rem}.space-x-1\.5 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.375rem * var(--tw-space-x-reverse));margin-left:calc(0.375rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-3 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.75rem * var(--tw-space-x-reverse));margin-left:calc(0.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(0.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(0.25rem * var(--tw-space-y-reverse))}.space-y-4 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-t{border-top-width:1px}.border-brandBlue-100{--tw-border-opacity:1;border-color:rgb(224 239 254 / var(--tw-border-opacity, 1))}.border-brandBlue-200{--tw-border-opacity:1;border-color:rgb(186 224 253 / var(--tw-border-opacity, 1))}.border-slate-100{--tw-border-opacity:1;border-color:rgb(241 245 249 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225 / var(--tw-border-opacity, 1))}.border-white\/20{border-color:rgb(255 255 255 / 0.2)}.border-white\/80{border-color:rgb(255 255 255 / 0.8)}.bg-\[\#06C755\]{--tw-bg-opacity:1;background-color:rgb(6 199 85 / var(--tw-bg-opacity, 1))}.bg-brandBlue-100{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.bg-brandBlue-50{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.bg-brandBlue-600{--tw-bg-opacity:1;background-color:rgb(0 114 198 / var(--tw-bg-opacity, 1))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-white\/10{background-color:rgb(255 255 255 / 0.1)}.bg-white\/40{background-color:rgb(255 255 255 / 0.4)}.bg-white\/60{background-color:rgb(255 255 255 / 0.6)}.bg-white\/70{background-color:rgb(255 255 255 / 0.7)}.bg-gradient-to-r{background-image:linear-gradient(to right, var(--tw-gradient-stops))}.bg-gradient-to-t{background-image:linear-gradient(to top, var(--tw-gradient-stops))}.from-brandBlue-600{--tw-gradient-from:#0072c6 var(--tw-gradient-from-position);--tw-gradient-to:rgb(0 114 198 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.from-slate-900\/40{--tw-gradient-from:rgb(15 23 42 / 0.4) var(--tw-gradient-from-position);--tw-gradient-to:rgb(15 23 42 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.to-brandBlue-800{--tw-gradient-to:#064e86 var(--tw-gradient-to-position)}.to-transparent{--tw-gradient-to:transparent var(--tw-gradient-to-position)}.object-cover{object-fit:cover}.p-3{padding:0.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-10{padding-left:2.5rem;padding-right:2.5rem}.px-3{padding-left:0.75rem;padding-right:0.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-1\.5{padding-top:0.375rem;padding-bottom:0.375rem}.py-2\.5{padding-top:0.625rem;padding-bottom:0.625rem}.py-3\.5{padding-top:0.875rem;padding-bottom:0.875rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-8{padding-top:2rem;padding-bottom:2rem}.pl-2{padding-left:0.5rem}.pt-6{padding-top:1.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-\[9px\]{font-size:9px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.font-black{font-weight:900}.font-bold{font-weight:700}.font-extrabold{font-weight:800}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-snug{line-height:1.375}.leading-tight{line-height:1.25}.tracking-wide{letter-spacing:0.025em}.tracking-wider{letter-spacing:0.05em}.tracking-widest{letter-spacing:0.1em}.text-brandBlue-200{--tw-text-opacity:1;color:rgb(186 224 253 / var(--tw-text-opacity, 1))}.text-brandBlue-50{--tw-text-opacity:1;color:rgb(240 247 255 / var(--tw-text-opacity, 1))}.text-brandBlue-600{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.text-brandBlue-700{--tw-text-opacity:1;color:rgb(2 91 162 / var(--tw-text-opacity, 1))}.text-green-100{--tw-text-opacity:1;color:rgb(220 252 231 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-slate-950{--tw-text-opacity:1;color:rgb(2 6 23 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-yellow-300{--tw-text-opacity:1;color:rgb(253 224 71 / var(--tw-text-opacity, 1))}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-md{--tw-shadow:0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-xl{--tw-shadow:0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.backdrop-blur-md{--tw-backdrop-blur:blur(12px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.duration-200{transition-duration:200ms}.duration-300{transition-duration:300ms}.duration-500{transition-duration:500ms}.hover\:scale-\[1\.02\]:hover{--tw-scale-x:1.02;--tw-scale-y:1.02;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:border-brandBlue-400:hover{--tw-border-opacity:1;border-color:rgb(56 171 248 / var(--tw-border-opacity, 1))}.hover\:bg-\[\#05b04b\]:hover{--tw-bg-opacity:1;background-color:rgb(5 176 75 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-100:hover{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-50:hover{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-700:hover{--tw-bg-opacity:1;background-color:rgb(2 91 162 / var(--tw-bg-opacity, 1))}.hover\:text-brandBlue-600:hover{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.group:hover .group-hover\:scale-105{--tw-scale-x:1.05;--tw-scale-y:1.05;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@media (min-width: 640px){.sm\:w-auto{width:auto}.sm\:grid-cols-3{grid-template-columns:repeat(3, minmax(0, 1fr))}}@media (min-width: 768px){.md\:col-span-5{grid-column:span 5 / span 5}.md\:col-span-7{grid-column:span 7 / span 7}.md\:aspect-square{aspect-ratio:1 / 1}.md\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}.md\:p-10{padding:2.5rem}.md\:p-12{padding:3rem}.md\:px-12{padding-left:3rem;padding-right:3rem}.md\:py-12{padding-top:3rem;padding-bottom:3rem}.md\:text-2xl{font-size:1.5rem;line-height:2rem}.md\:text-3xl{font-size:1.875rem;line-height:2.25rem}.md\:text-4xl{font-size:2.25rem;line-height:2.5rem}.md\:text-lg{font-size:1.125rem;line-height:1.75rem}.md\:text-sm{font-size:0.875rem;line-height:1.25rem}}</style><style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:Inter, Noto Sans TC, sans-serif;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.pointer-events-none{pointer-events:none}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.inset-0{inset:0px}.left-1\/2{left:50%}.top-8{top:2rem}.z-10{z-index:10}.z-20{z-index:20}.z-50{z-index:50}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-2{margin-bottom:0.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mr-1{margin-right:0.25rem}.mr-2{margin-right:0.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.grid{display:grid}.aspect-\[4\/3\]{aspect-ratio:4/3}.h-1\.5{height:0.375rem}.h-16{height:4rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-1\/5{width:20%}.w-16{width:4rem}.w-8{width:2rem}.w-full{width:100%}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1\/2{--tw-translate-x:-50%;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-0{--tw-translate-y:0px;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;user-select:none}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-3{gap:0.75rem}.gap-8{gap:2rem}.space-x-1\.5 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.375rem * var(--tw-space-x-reverse));margin-left:calc(0.375rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-3 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.75rem * var(--tw-space-x-reverse));margin-left:calc(0.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(0.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(0.25rem * var(--tw-space-y-reverse))}.space-y-4 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-t{border-top-width:1px}.border-brandBlue-100{--tw-border-opacity:1;border-color:rgb(224 239 254 / var(--tw-border-opacity, 1))}.border-brandBlue-200{--tw-border-opacity:1;border-color:rgb(186 224 253 / var(--tw-border-opacity, 1))}.border-slate-100{--tw-border-opacity:1;border-color:rgb(241 245 249 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225 / var(--tw-border-opacity, 1))}.border-white\/20{border-color:rgb(255 255 255 / 0.2)}.border-white\/80{border-color:rgb(255 255 255 / 0.8)}.bg-\[\#06C755\]{--tw-bg-opacity:1;background-color:rgb(6 199 85 / var(--tw-bg-opacity, 1))}.bg-brandBlue-100{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.bg-brandBlue-50{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.bg-brandBlue-600{--tw-bg-opacity:1;background-color:rgb(0 114 198 / var(--tw-bg-opacity, 1))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-white\/10{background-color:rgb(255 255 255 / 0.1)}.bg-white\/40{background-color:rgb(255 255 255 / 0.4)}.bg-white\/60{background-color:rgb(255 255 255 / 0.6)}.bg-white\/70{background-color:rgb(255 255 255 / 0.7)}.bg-gradient-to-r{background-image:linear-gradient(to right, var(--tw-gradient-stops))}.bg-gradient-to-t{background-image:linear-gradient(to top, var(--tw-gradient-stops))}.from-brandBlue-600{--tw-gradient-from:#0072c6 var(--tw-gradient-from-position);--tw-gradient-to:rgb(0 114 198 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.from-slate-900\/40{--tw-gradient-from:rgb(15 23 42 / 0.4) var(--tw-gradient-from-position);--tw-gradient-to:rgb(15 23 42 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.to-brandBlue-800{--tw-gradient-to:#064e86 var(--tw-gradient-to-position)}.to-transparent{--tw-gradient-to:transparent var(--tw-gradient-to-position)}.object-cover{object-fit:cover}.p-3{padding:0.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-10{padding-left:2.5rem;padding-right:2.5rem}.px-3{padding-left:0.75rem;padding-right:0.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-1\.5{padding-top:0.375rem;padding-bottom:0.375rem}.py-2\.5{padding-top:0.625rem;padding-bottom:0.625rem}.py-3\.5{padding-top:0.875rem;padding-bottom:0.875rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-8{padding-top:2rem;padding-bottom:2rem}.pl-2{padding-left:0.5rem}.pt-6{padding-top:1.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-\[9px\]{font-size:9px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.font-black{font-weight:900}.font-bold{font-weight:700}.font-extrabold{font-weight:800}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-snug{line-height:1.375}.leading-tight{line-height:1.25}.tracking-wide{letter-spacing:0.025em}.tracking-wider{letter-spacing:0.05em}.tracking-widest{letter-spacing:0.1em}.text-brandBlue-200{--tw-text-opacity:1;color:rgb(186 224 253 / var(--tw-text-opacity, 1))}.text-brandBlue-50{--tw-text-opacity:1;color:rgb(240 247 255 / var(--tw-text-opacity, 1))}.text-brandBlue-600{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.text-brandBlue-700{--tw-text-opacity:1;color:rgb(2 91 162 / var(--tw-text-opacity, 1))}.text-green-100{--tw-text-opacity:1;color:rgb(220 252 231 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-slate-950{--tw-text-opacity:1;color:rgb(2 6 23 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-yellow-300{--tw-text-opacity:1;color:rgb(253 224 71 / var(--tw-text-opacity, 1))}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-md{--tw-shadow:0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-xl{--tw-shadow:0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.backdrop-blur-md{--tw-backdrop-blur:blur(12px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.duration-200{transition-duration:200ms}.duration-300{transition-duration:300ms}.duration-500{transition-duration:500ms}.hover\:scale-\[1\.02\]:hover{--tw-scale-x:1.02;--tw-scale-y:1.02;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:border-brandBlue-400:hover{--tw-border-opacity:1;border-color:rgb(56 171 248 / var(--tw-border-opacity, 1))}.hover\:bg-\[\#05b04b\]:hover{--tw-bg-opacity:1;background-color:rgb(5 176 75 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-100:hover{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-50:hover{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-700:hover{--tw-bg-opacity:1;background-color:rgb(2 91 162 / var(--tw-bg-opacity, 1))}.hover\:text-brandBlue-600:hover{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.group:hover .group-hover\:scale-105{--tw-scale-x:1.05;--tw-scale-y:1.05;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@media (min-width: 640px){.sm\:w-auto{width:auto}.sm\:grid-cols-3{grid-template-columns:repeat(3, minmax(0, 1fr))}}@media (min-width: 768px){.md\:col-span-5{grid-column:span 5 / span 5}.md\:col-span-7{grid-column:span 7 / span 7}.md\:aspect-square{aspect-ratio:1 / 1}.md\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}.md\:p-10{padding:2.5rem}.md\:p-12{padding:3rem}.md\:px-12{padding-left:3rem;padding-right:3rem}.md\:py-12{padding-top:3rem;padding-bottom:3rem}.md\:text-2xl{font-size:1.5rem;line-height:2rem}.md\:text-3xl{font-size:1.875rem;line-height:2.25rem}.md\:text-4xl{font-size:2.25rem;line-height:2.5rem}.md\:text-lg{font-size:1.125rem;line-height:1.75rem}.md\:text-sm{font-size:0.875rem;line-height:1.25rem}}</style><style>*, ::before, ::after{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-gradient-from-position: ;--tw-gradient-via-position: ;--tw-gradient-to-position: ;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:rgb(59 130 246 / 0.5);--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: ;--tw-contain-size: ;--tw-contain-layout: ;--tw-contain-paint: ;--tw-contain-style: }/* ! tailwindcss v3.4.17 | MIT License | https://tailwindcss.com */*,::after,::before{box-sizing:border-box;border-width:0;border-style:solid;border-color:#e5e7eb}::after,::before{--tw-content:''}:host,html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;tab-size:4;font-family:Inter, Noto Sans TC, sans-serif;font-feature-settings:normal;font-variation-settings:normal;-webkit-tap-highlight-color:transparent}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;font-feature-settings:normal;font-variation-settings:normal;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:baseline}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-feature-settings:inherit;font-variation-settings:inherit;font-size:100%;font-weight:inherit;line-height:inherit;letter-spacing:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}button,input:where([type=button]),input:where([type=reset]),input:where([type=submit]){-webkit-appearance:button;background-color:transparent;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:baseline}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0;padding:0}legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}dialog{padding:0}textarea{resize:vertical}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]:where(:not([hidden=until-found])){display:none}.pointer-events-none{pointer-events:none}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.inset-0{inset:0px}.left-1\/2{left:50%}.top-8{top:2rem}.z-10{z-index:10}.z-20{z-index:20}.z-50{z-index:50}.mx-auto{margin-left:auto;margin-right:auto}.mb-1{margin-bottom:0.25rem}.mb-2{margin-bottom:0.5rem}.mb-4{margin-bottom:1rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.mr-1{margin-right:0.25rem}.mr-2{margin-right:0.5rem}.mt-4{margin-top:1rem}.mt-8{margin-top:2rem}.block{display:block}.flex{display:flex}.inline-flex{display:inline-flex}.grid{display:grid}.aspect-\[4\/3\]{aspect-ratio:4/3}.h-1\.5{height:0.375rem}.h-16{height:4rem}.h-8{height:2rem}.h-full{height:100%}.min-h-screen{min-height:100vh}.w-1\/5{width:20%}.w-16{width:4rem}.w-8{width:2rem}.w-full{width:100%}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.flex-shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.-translate-x-1\/2{--tw-translate-x:-50%;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-0{--tw-translate-y:0px;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.select-none{-webkit-user-select:none;user-select:none}.grid-cols-1{grid-template-columns:repeat(1, minmax(0, 1fr))}.flex-col{flex-direction:column}.flex-wrap{flex-wrap:wrap}.items-center{align-items:center}.justify-center{justify-content:center}.justify-between{justify-content:space-between}.gap-2{gap:0.5rem}.gap-3{gap:0.75rem}.gap-8{gap:2rem}.space-x-1\.5 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.375rem * var(--tw-space-x-reverse));margin-left:calc(0.375rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-2 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.5rem * var(--tw-space-x-reverse));margin-left:calc(0.5rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-3 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(0.75rem * var(--tw-space-x-reverse));margin-left:calc(0.75rem * calc(1 - var(--tw-space-x-reverse)))}.space-x-4 > :not([hidden]) ~ :not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem * var(--tw-space-x-reverse));margin-left:calc(1rem * calc(1 - var(--tw-space-x-reverse)))}.space-y-1 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(0.25rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(0.25rem * var(--tw-space-y-reverse))}.space-y-4 > :not([hidden]) ~ :not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem * calc(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem * var(--tw-space-y-reverse))}.overflow-hidden{overflow:hidden}.rounded-2xl{border-radius:1rem}.rounded-3xl{border-radius:1.5rem}.rounded-full{border-radius:9999px}.rounded-lg{border-radius:0.5rem}.rounded-xl{border-radius:0.75rem}.border{border-width:1px}.border-b{border-bottom-width:1px}.border-l{border-left-width:1px}.border-t{border-top-width:1px}.border-brandBlue-100{--tw-border-opacity:1;border-color:rgb(224 239 254 / var(--tw-border-opacity, 1))}.border-brandBlue-200{--tw-border-opacity:1;border-color:rgb(186 224 253 / var(--tw-border-opacity, 1))}.border-slate-100{--tw-border-opacity:1;border-color:rgb(241 245 249 / var(--tw-border-opacity, 1))}.border-slate-200{--tw-border-opacity:1;border-color:rgb(226 232 240 / var(--tw-border-opacity, 1))}.border-slate-300{--tw-border-opacity:1;border-color:rgb(203 213 225 / var(--tw-border-opacity, 1))}.border-white\/20{border-color:rgb(255 255 255 / 0.2)}.border-white\/80{border-color:rgb(255 255 255 / 0.8)}.bg-\[\#06C755\]{--tw-bg-opacity:1;background-color:rgb(6 199 85 / var(--tw-bg-opacity, 1))}.bg-brandBlue-100{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.bg-brandBlue-50{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.bg-brandBlue-600{--tw-bg-opacity:1;background-color:rgb(0 114 198 / var(--tw-bg-opacity, 1))}.bg-slate-100{--tw-bg-opacity:1;background-color:rgb(241 245 249 / var(--tw-bg-opacity, 1))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255 / var(--tw-bg-opacity, 1))}.bg-white\/10{background-color:rgb(255 255 255 / 0.1)}.bg-white\/40{background-color:rgb(255 255 255 / 0.4)}.bg-white\/60{background-color:rgb(255 255 255 / 0.6)}.bg-white\/70{background-color:rgb(255 255 255 / 0.7)}.bg-gradient-to-r{background-image:linear-gradient(to right, var(--tw-gradient-stops))}.bg-gradient-to-t{background-image:linear-gradient(to top, var(--tw-gradient-stops))}.from-brandBlue-600{--tw-gradient-from:#0072c6 var(--tw-gradient-from-position);--tw-gradient-to:rgb(0 114 198 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.from-slate-900\/40{--tw-gradient-from:rgb(15 23 42 / 0.4) var(--tw-gradient-from-position);--tw-gradient-to:rgb(15 23 42 / 0) var(--tw-gradient-to-position);--tw-gradient-stops:var(--tw-gradient-from), var(--tw-gradient-to)}.to-brandBlue-800{--tw-gradient-to:#064e86 var(--tw-gradient-to-position)}.to-transparent{--tw-gradient-to:transparent var(--tw-gradient-to-position)}.object-cover{object-fit:cover}.p-3{padding:0.75rem}.p-4{padding:1rem}.p-6{padding:1.5rem}.p-8{padding:2rem}.px-10{padding-left:2.5rem;padding-right:2.5rem}.px-3{padding-left:0.75rem;padding-right:0.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-5{padding-left:1.25rem;padding-right:1.25rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.py-1\.5{padding-top:0.375rem;padding-bottom:0.375rem}.py-2\.5{padding-top:0.625rem;padding-bottom:0.625rem}.py-3\.5{padding-top:0.875rem;padding-bottom:0.875rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-8{padding-top:2rem;padding-bottom:2rem}.pl-2{padding-left:0.5rem}.pt-6{padding-top:1.5rem}.text-left{text-align:left}.text-center{text-align:center}.text-2xl{font-size:1.5rem;line-height:2rem}.text-3xl{font-size:1.875rem;line-height:2.25rem}.text-\[9px\]{font-size:9px}.text-base{font-size:1rem;line-height:1.5rem}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:0.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:0.75rem;line-height:1rem}.font-black{font-weight:900}.font-bold{font-weight:700}.font-extrabold{font-weight:800}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.leading-relaxed{line-height:1.625}.leading-snug{line-height:1.375}.leading-tight{line-height:1.25}.tracking-wide{letter-spacing:0.025em}.tracking-wider{letter-spacing:0.05em}.tracking-widest{letter-spacing:0.1em}.text-brandBlue-200{--tw-text-opacity:1;color:rgb(186 224 253 / var(--tw-text-opacity, 1))}.text-brandBlue-50{--tw-text-opacity:1;color:rgb(240 247 255 / var(--tw-text-opacity, 1))}.text-brandBlue-600{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.text-brandBlue-700{--tw-text-opacity:1;color:rgb(2 91 162 / var(--tw-text-opacity, 1))}.text-green-100{--tw-text-opacity:1;color:rgb(220 252 231 / var(--tw-text-opacity, 1))}.text-slate-500{--tw-text-opacity:1;color:rgb(100 116 139 / var(--tw-text-opacity, 1))}.text-slate-600{--tw-text-opacity:1;color:rgb(71 85 105 / var(--tw-text-opacity, 1))}.text-slate-700{--tw-text-opacity:1;color:rgb(51 65 85 / var(--tw-text-opacity, 1))}.text-slate-800{--tw-text-opacity:1;color:rgb(30 41 59 / var(--tw-text-opacity, 1))}.text-slate-900{--tw-text-opacity:1;color:rgb(15 23 42 / var(--tw-text-opacity, 1))}.text-slate-950{--tw-text-opacity:1;color:rgb(2 6 23 / var(--tw-text-opacity, 1))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255 / var(--tw-text-opacity, 1))}.text-yellow-300{--tw-text-opacity:1;color:rgb(253 224 71 / var(--tw-text-opacity, 1))}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color), 0 1px 2px -1px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-md{--tw-shadow:0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.shadow-xl{--tw-shadow:0 20px 25px -5px rgb(0 0 0 / 0.1), 0 8px 10px -6px rgb(0 0 0 / 0.1);--tw-shadow-colored:0 20px 25px -5px var(--tw-shadow-color), 0 8px 10px -6px var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow)}.backdrop-blur-md{--tw-backdrop-blur:blur(12px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-colors{transition-property:color, background-color, border-color, fill, stroke, -webkit-text-decoration-color;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke;transition-property:color, background-color, border-color, text-decoration-color, fill, stroke, -webkit-text-decoration-color;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.transition-transform{transition-property:transform;transition-timing-function:cubic-bezier(0.4, 0, 0.2, 1);transition-duration:150ms}.duration-200{transition-duration:200ms}.duration-300{transition-duration:300ms}.duration-500{transition-duration:500ms}.hover\:scale-\[1\.02\]:hover{--tw-scale-x:1.02;--tw-scale-y:1.02;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.hover\:border-brandBlue-400:hover{--tw-border-opacity:1;border-color:rgb(56 171 248 / var(--tw-border-opacity, 1))}.hover\:bg-\[\#05b04b\]:hover{--tw-bg-opacity:1;background-color:rgb(5 176 75 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-100:hover{--tw-bg-opacity:1;background-color:rgb(224 239 254 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-50:hover{--tw-bg-opacity:1;background-color:rgb(240 247 255 / var(--tw-bg-opacity, 1))}.hover\:bg-brandBlue-700:hover{--tw-bg-opacity:1;background-color:rgb(2 91 162 / var(--tw-bg-opacity, 1))}.hover\:text-brandBlue-600:hover{--tw-text-opacity:1;color:rgb(0 114 198 / var(--tw-text-opacity, 1))}.group:hover .group-hover\:scale-105{--tw-scale-x:1.05;--tw-scale-y:1.05;transform:translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@media (min-width: 640px){.sm\:w-auto{width:auto}.sm\:grid-cols-3{grid-template-columns:repeat(3, minmax(0, 1fr))}}@media (min-width: 768px){.md\:col-span-5{grid-column:span 5 / span 5}.md\:col-span-7{grid-column:span 7 / span 7}.md\:aspect-square{aspect-ratio:1 / 1}.md\:grid-cols-12{grid-template-columns:repeat(12, minmax(0, 1fr))}.md\:p-10{padding:2.5rem}.md\:p-12{padding:3rem}.md\:px-12{padding-left:3rem;padding-right:3rem}.md\:py-12{padding-top:3rem;padding-bottom:3rem}.md\:text-2xl{font-size:1.5rem;line-height:2rem}.md\:text-3xl{font-size:1.875rem;line-height:2.25rem}.md\:text-4xl{font-size:2.25rem;line-height:2.5rem}.md\:text-lg{font-size:1.125rem;line-height:1.75rem}.md\:text-sm{font-size:0.875rem;line-height:1.25rem}}</style><style id="tag-inspector-styles">
                    .inspector-hover-outline { outline: 1px dotted #dc3545 !important; box-shadow: inset 0 0 0 1px #dc3545; }
                    #tag-inspector-tooltip { position: fixed; display: none; background-color: #dc3545; color: white; padding: 2px 6px; font-size: 12px; border-radius: 4px; pointer-events: none; z-index: 9999; font-family: monospace; }
                </style></head>
<body class="text-slate-900 min-h-screen flex flex-col justify-between select-none" contenteditable="true">

    <!-- 3D Canvas fixed background -->
    <div id="webgl-container"></div>

    <header class="w-full py-4 px-6 md:px-12 flex justify-between items-center z-20 relative bg-white/60 backdrop-blur-md border-b border-brandBlue-100">
        <div class="flex items-center space-x-2">
            <span class="text-brandBlue-600 font-black text-xl md:text-2xl tracking-wider">HouseStyle</span>
            <span class="text-slate-800 font-medium text-sm md:text-md border-l border-slate-300 pl-2">好時代衛浴</span>
        </div>
        <div class="text-xs md:text-sm font-semibold tracking-widest text-brandBlue-700 uppercase bg-brandBlue-50 px-3 py-1.5 rounded-full border border-brandBlue-100">
            父親節美學企劃
        </div>
    </header>

    <main class="flex-grow flex items-center justify-center px-4 py-8 md:py-12 z-10 relative">
        <div class="w-full max-w-4xl">

            <!-- 1. INTRO SCREEN -->
            <div id="intro-screen" class="hide-page">
                <div class="glass-panel p-8 md:p-12 rounded-3xl text-center max-w-2xl mx-auto border border-white/80">
                    <div class="w-16 h-16 bg-brandBlue-100 rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fa-solid fa-bath text-brandBlue-600 text-2xl"></i>
                    </div>
                    <h1 class="text-3xl md:text-4xl font-bold text-slate-950 mb-4 tracking-wide leading-tight">
                        測出最適合你的浴室設計🛁</h1>
                    <p class="text-brandBlue-600 text-sm md:text-md tracking-widest font-semibold uppercase mb-6">
                        找尋專屬你的衛浴美學風格
                    </p>
                    <p class="text-slate-600 text-base md:text-lg mb-8 leading-relaxed">
                        家是卸下武裝的城堡，而浴室是唯一的絕對私密聖地。<br>
                        只需兩分鐘，探索你在洗沐時光中最真實的靈魂偏好，<br>
                        解鎖最契合你日常的衛浴設計，並獲取父親節限定豪禮！
                    </p>
                    <button onclick="startQuiz()" class="btn-glow w-full sm:w-auto bg-brandBlue-600 hover:bg-brandBlue-700 text-white font-semibold text-lg py-4 px-10 rounded-full inline-flex items-center justify-center space-x-3 shadow-lg">
                        <span class="">開啟衛浴空間之旅</span>
                        <i class="fa-solid fa-arrow-right"></i>
                    </button>
                </div>
            </div>

            <!-- 2. QUIZ SCREEN -->
            <div id="quiz-screen" class="hide-page" style="opacity: 0.3; transform: translateY(10px);">
                <div class="glass-panel p-6 md:p-10 rounded-3xl w-full max-w-2xl mx-auto border border-white/80 relative">
                    <!-- Progress meter -->
                    <div class="flex justify-between items-center mb-6">
                        <span id="quiz-step-text" class="text-xs font-bold tracking-widest text-brandBlue-600 uppercase">QUESTION 05</span>
                        <span id="quiz-progress-text" class="text-xs font-bold text-slate-500">5 / 5</span>
                    </div>
                    <div class="w-full bg-brandBlue-100 h-1.5 rounded-full overflow-hidden mb-8">
                        <div id="progress-bar" class="bg-brandBlue-600 h-full w-1/5 transition-all duration-300" style="width: 100%;"></div>
                    </div>

                    <!-- Question Container -->
                    <h2 id="question-text" class="text-xl md:text-2xl font-bold text-slate-950 mb-8 leading-snug">看到下面哪一句最符合你的生活態度？</h2>

                    <!-- Options Container -->
                    <div class="space-y-4">
                        <button onclick="selectOption('A')" class="w-full text-left p-4 rounded-2xl bg-white/70 hover:bg-brandBlue-50 border border-slate-200 hover:border-brandBlue-400 text-slate-800 font-medium text-md flex items-center space-x-4 transition-all duration-200">
                            <span class="flex-shrink-0 w-8 h-8 rounded-full bg-slate-100 text-slate-600 text-sm font-bold flex items-center justify-center border border-slate-200">A</span>
                            <span id="opt-text-A" class="">簡單有效率，就是最好的設計。</span>
                        </button>
                        <button onclick="selectOption('B')" class="w-full text-left p-4 rounded-2xl bg-white/70 hover:bg-brandBlue-50 border border-slate-200 hover:border-brandBlue-400 text-slate-800 font-medium text-md flex items-center space-x-4 transition-all duration-200">
                            <span class="flex-shrink-0 w-8 h-8 rounded-full bg-slate-100 text-slate-600 text-sm font-bold flex items-center justify-center border border-slate-200">B</span>
                            <span id="opt-text-B" class="">生活要有質感，才能享受人生。</span>
                        </button>
                        <button onclick="selectOption('C')" class="w-full text-left p-4 rounded-2xl bg-white/70 hover:bg-brandBlue-50 border border-slate-200 hover:border-brandBlue-400 text-slate-800 font-medium text-md flex items-center space-x-4 transition-all duration-200">
                            <span class="flex-shrink-0 w-8 h-8 rounded-full bg-slate-100 text-slate-600 text-sm font-bold flex items-center justify-center border border-slate-200">C</span>
                            <span id="opt-text-C" class="">少一點、多剛好。</span>
                        </button>
                        <button onclick="selectOption('D')" class="w-full text-left p-4 rounded-2xl bg-white/70 hover:bg-brandBlue-50 border border-slate-200 hover:border-brandBlue-400 text-slate-800 font-medium text-md flex items-center space-x-4 transition-all duration-200">
                            <span class="flex-shrink-0 w-8 h-8 rounded-full bg-slate-100 text-slate-600 text-sm font-bold flex items-center justify-center border border-slate-200">D</span>
                            <span id="opt-text-D">美感就是生活的一部分。</span>
                        </button>
                        <button onclick="selectOption('E')" class="w-full text-left p-4 rounded-2xl bg-white/70 hover:bg-brandBlue-50 border border-slate-200 hover:border-brandBlue-400 text-slate-800 font-medium text-md flex items-center space-x-4 transition-all duration-200">
                            <span class="flex-shrink-0 w-8 h-8 rounded-full bg-slate-100 text-slate-600 text-sm font-bold flex items-center justify-center border border-slate-200">E</span>
                            <span id="opt-text-E">舒服，比什麼都重要。</span>
                        </button>
                    </div>
                </div>
            </div>

            <!-- 3. RESULT SCREEN -->
            <div id="result-screen" class="show-page">
                <div class="glass-panel p-6 md:p-10 rounded-3xl w-full max-w-3xl mx-auto border border-white/80">
                    <div class="text-center mb-6">
                        <span class="text-xs font-black tracking-widest text-brandBlue-600 uppercase bg-brandBlue-100 px-4 py-1.5 rounded-full">YOUR STYLE RESULT</span>
                        <h2 class="text-2xl md:text-3xl font-bold text-slate-950 mt-4">專屬你的浴室美學風格</h2>
                    </div>

                    <!-- Split layout: Image & Result Details -->
                    <div class="grid grid-cols-1 md:grid-cols-12 gap-8 items-center mb-8">
                        <!-- Dynamic Style Image -->
                        <div class="md:col-span-5 relative group overflow-hidden rounded-2xl shadow-md bg-slate-100 aspect-[4/3] md:aspect-square flex items-center justify-center">
                            <img id="style-image" src="https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?q=80&amp;w=800&amp;auto=format&amp;fit=crop" alt="風格照片" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" onerror="this.src='https://placehold.co/600x600/e2e8f0/0f172a?text=HouseStyle+Bath'" style="opacity: 1;">
                            <div class="absolute inset-0 bg-gradient-to-t from-slate-900/40 to-transparent"></div>
                        </div>

                        <!-- Style details -->
                        <div class="md:col-span-7 space-y-4">
                            <h3 id="result-style-title" class="text-2xl md:text-3xl font-extrabold text-brandBlue-600 flex items-center gap-2">飯店精品風 ⭐</h3>
                            <p id="result-style-desc" class="text-slate-700 text-base leading-relaxed">你喜歡有質感、有層次的生活，重視空間帶來的享受感，適合打造五星級飯店般的衛浴。在低調而奢華的色調下，品味專屬的極致洗沐時光。</p>
                            
                            <div class="bg-brandBlue-50 border border-brandBlue-100 p-4 rounded-xl">
                                <span class="text-xs font-bold text-brandBlue-700 block mb-1 tracking-wider uppercase">適合配置與材質：</span>
                                <p id="result-style-materials" class="text-slate-800 font-medium text-sm">石紋磁磚、大面鏡櫃、間接照明、黑白灰色系五金套裝。</p>
                            </div>
                        </div>
                    </div>

                    <!-- Promotion box -->
                    <div class="bg-gradient-to-r from-brandBlue-600 to-brandBlue-800 text-white rounded-2xl p-6 mb-8 shadow-md">
                        <h4 class="text-lg font-bold mb-2 flex items-center gap-2">
                            <i class="fa-solid fa-ribbon text-yellow-300"></i> 好時代 7-8 月父親節特別獻禮
                        </h4>
                        <p id="result-promo-offer" class="text-sm text-brandBlue-50 leading-relaxed mb-4"><i class="fa-solid fa-gift mr-2"></i> 憑此畫面預約好時代門市諮詢，升級專屬「精品級極簡 L 型乾濕分離滑門」享父親節特別特惠價，加碼免加價贈送多功能防霧鏡櫃！</p>
                        
                        <!-- Coupon field -->
                        <div class="bg-white/10 backdrop-blur-md rounded-xl p-3 flex flex-wrap items-center justify-between gap-3 border border-white/20">
                            <div class="">
                                <span class="text-xs text-brandBlue-200 block">風格專屬優惠代碼</span>
                                <span id="style-code" class="text-xl font-bold tracking-widest text-white">HS-DAD88-HOTEL</span>
                            </div>
                            <button onclick="copyStyleCode()" class="bg-white hover:bg-brandBlue-100 text-brandBlue-700 px-5 py-2.5 rounded-lg text-sm font-bold flex items-center space-x-2 transition-colors duration-200 shadow">
                                <i id="copy-icon" class="fa-regular fa-copy"></i>
                                <span>複製代碼</span>
                            </button>
                        </div>
                    </div>

                    <!-- Action buttons (Split 3 ways for local LINE@ redirects) -->
                    <div class="space-y-4">
                        <div class="text-center">
                            <span class="text-xs font-bold tracking-wider text-slate-500 uppercase block mb-2">✦ 點擊下方門市加入LINE官方帳號 ✦</span>
                        </div>
                        <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                            <button onclick="handleLineRedirect('taipei')" class="w-full py-3.5 px-4 rounded-xl bg-[#06C755] hover:bg-[#05b04b] text-white font-bold text-xs flex flex-col items-center justify-center space-y-1 transition-all duration-200 shadow-md hover:scale-[1.02]">
                                <div class="flex items-center space-x-1.5">
                                    <i class="fa-brands fa-line text-lg"></i>
                                    <span class="text-sm">台北門市 預約</span>
                                </div>
                                <span class="text-[9px] text-green-100 font-normal"></span>
                            </button>
                            <button onclick="handleLineRedirect('taoyuan')" class="w-full py-3.5 px-4 rounded-xl bg-[#06C755] hover:bg-[#05b04b] text-white font-bold text-xs flex flex-col items-center justify-center space-y-1 transition-all duration-200 shadow-md hover:scale-[1.02]">
                                <div class="flex items-center space-x-1.5">
                                    <i class="fa-brands fa-line text-lg"></i>
                                    <span class="text-sm">桃園門市 預約</span>
                                </div>
                                <span class="text-[9px] text-green-100 font-normal"></span>
                            </button>
                            <button onclick="handleLineRedirect('hsinchu')" class="w-full py-3.5 px-4 rounded-xl bg-[#06C755] hover:bg-[#05b04b] text-white font-bold text-xs flex flex-col items-center justify-center space-y-1 transition-all duration-200 shadow-md hover:scale-[1.02]">
                                <div class="flex items-center space-x-1.5">
                                    <i class="fa-brands fa-line text-lg"></i>
                                    <span class="text-sm">新竹門市 預約</span>
                                </div>
                                <span class="text-[9px] text-green-100 font-normal"></span>
                            </button>
             </div>
<!-- Restart button -->
<div class="mt-8 border-t border-slate-100 pt-6">
    <center class="">
        <button onclick="restartQuiz()" class="text-slate-500 hover:text-brandBlue-600 font-bold text-sm transition-colors duration-200">
            <i class="fa-solid fa-rotate-left mr-1"></i>
            重新測驗
        </button>
    </center>
</div>        
                </div>
            </div>

        </div>
    </div></main>

    <!-- Global Floating Feedback Toast -->
    <div id="toast-message" class="fixed top-8 left-1/2 -translate-x-1/2 z-50 glass-panel border-brandBlue-200 py-3.5 px-6 rounded-full text-brandBlue-700 font-semibold text-sm flex items-center space-x-2 shadow-xl opacity-0 translate-y-0 transition-all duration-300 pointer-events-none">
        <i class="fa-solid fa-check text-brandBlue-600"></i>
        <span>優惠代碼已成功複製！</span>
    </div>

    <!-- Footer copyright info -->
    <footer class="w-full py-4 text-center text-xs text-slate-500 border-t border-brandBlue-100 bg-white/40 z-10 relative">
        © 2026 HouseStyle 好時代衛浴 版權所有. 專業到府丈量與浴室櫃體訂製服務.
    </footer>

    <script>
        // --- 5-QUESTION MULTIPLE CHOICE DATA (REORDERED FOR LOGICAL CONVERSION) ---
        // Option Keys (A, B, C, D, E) point to different styles in each question to ensure variety
        const quizData = [
            {
                id: 1,
                question: "如果今天終於放假，你最想怎麼度過？",
                options: {
                    A: { text: "到山上、森林或咖啡廳放空", style: 'B' }, // Nordic
                    B: { text: "約朋友吃早午餐、拍美照", style: 'D' }, // Creamy
                    C: { text: "去五星級飯店住一晚", style: 'A' },     // Hotel
                    D: { text: "在家泡茶、看書、放空", style: 'E' },     // Muji
                    E: { text: "把家裡整理得乾乾淨淨", style: 'C' }     // Modern
                }
            },
            {
                id: 2,
                question: "你最不能接受浴室出現什麼情況？",
                options: {
                    A: { text: "東西亂放、收納不足", style: 'C' },     // Modern
                    B: { text: "看起來沒有質感", style: 'A' },         // Hotel
                    C: { text: "空間讓人覺得壓迫、吵雜", style: 'E' },     // Muji
                    D: { text: "光線昏暗、沒有溫度", style: 'B' },     // Nordic
                    E: { text: "配色不好看、不夠有設計感", style: 'D' } // Creamy
                }
            },
            {
                id: 3,
                question: "如果重新裝潢浴室，你最想投資哪一項？",
                options: {
                    A: { text: "簡約耐看的整體空間", style: 'E' },     // Muji
                    B: { text: "收納設計與乾濕分離", style: 'C' },     // Modern
                    C: { text: "漂亮的磁磚與造型五金", style: 'D' }, // Creamy
                    D: { text: "飯店等級設備", style: 'A' },         // Hotel
                    E: { text: "木質浴櫃與舒服燈光", style: 'B' }     // Nordic
                }
            },
            {
                id: 4,
                question: "你希望每天走進浴室的第一個感受是？",
                options: {
                    A: { text: "很漂亮，很有品味。", style: 'D' },     // Creamy
                    B: { text: "很安靜，很療癒。", style: 'E' },         // Muji
                    C: { text: "很舒服，很放鬆。", style: 'B' },         // Nordic
                    D: { text: "很乾淨，很俐落。", style: 'C' },         // Modern
                    E: { text: "哇，好像精品飯店。", style: 'A' }         // Hotel
                }
            },
            {
                id: 5,
                question: "看到下面哪一句最符合你的生活態度？",
                options: {
                    A: { text: "簡單有效率，就是最好的設計。", style: 'C' }, // Modern
                    B: { text: "生活要有質感，才能享受人生。", style: 'A' }, // Hotel
                    C: { text: "少一點、多剛好。", style: 'E' },         // Muji
                    D: { text: "美感就是生活的一部分。", style: 'D' },     // Creamy
                    E: { text: "舒服，比什麼都重要。", style: 'B' }         // Nordic
                }
            }
        ];

        const styleMetadata = {
            'A': {
                title: "飯店精品風 ⭐",
                desc: "你喜歡有質感、有層次的生活，重視空間帶來的享受感，適合打造五星級飯店般的衛浴。在低調而奢華的色調下，品味專屬的極致洗沐時光。",
                materials: "石紋磁磚、大面鏡櫃、間接照明、黑白灰色系五金套裝。",
                promo: "憑此畫面預約好時代門市諮詢，可享父親節特別豪禮！",
                code: "HS-DAD88-HOTEL",
                image: "https://images.unsplash.com/photo-1552321554-5fefe8c9ef14?q=80&w=800&auto=format&fit=crop"
            },
            'B': {
                title: "北歐自然風 🌿",
                desc: "你追求舒適與放鬆，喜歡自然元素與溫暖色調，打造療癒感衛浴最適合你。大量的留白與溫馨的大地色系，一洗整天的喧囂與壓力。",
                materials: "木紋浴櫃、淺色磁磚、自然採光、奶油色系配件。",
                promo: "憑此畫面預約好時代門市諮詢，可享父親節特別豪禮！",
                code: "HS-DAD88-NORDIC",
                image: "https://images.unsplash.com/photo-1584622650111-993a426fbf0a?q=80&w=800&auto=format&fit=crop"
            },
            'C': {
                title: "現代極簡風 📐",
                desc: "你重視機能與收納，喜歡乾淨俐落的空間，實用與美感兼具才是你的理想衛浴。利用隱藏式收納與俐落線條，創造無雜訊的絕對領域。",
                materials: "隱藏收納、無把手浴櫃、玻璃隔間、灰白色系搭配。",
                promo: "憑此畫面預約好時代門市諮詢，可享父親節特別豪禮！",
                code: "HS-DAD88-MODERN",
                image: "https://images.unsplash.com/photo-1600566752355-35792bedcfea?q=80&w=800&auto=format&fit=crop"
            },
            'D': {
                title: "奶油輕奢風 🍦",
                desc: "你喜歡柔和、有設計感的生活氛圍，希望每天都能在漂亮的空間中開始與結束一天。精緻的金邊與溫柔的弧形造型，點亮極致美學生活。",
                materials: "米白色漆、弧形設計浴櫃、金色五金件、柔光防霧鏡燈。",
                promo: "憑此畫面預約好時代門市諮詢，可享父親節特別豪禮！",
                code: "HS-DAD88-CREAMY",
                image: "https://images.unsplash.com/photo-1620626011761-996317b6979a?q=80&w=800&auto=format&fit=crop"
            },
            'E': {
                title: "日式無印風 🍵",
                desc: "你偏好簡單、安靜、耐看的設計，重視留白與自然材質，讓浴室成為最放鬆的角落。不盲從奢華，更偏好與內心平靜的誠摯對話。",
                materials: "木紋色櫃體、簡約收納方式、柔和低溫照明。",
                promo: "憑此畫面預約好時代門市諮詢，可享父親節特別豪禮！",
                code: "HS-DAD88-MUJI",
                image: "https://images.unsplash.com/photo-1618221195710-dd6b41faaea6?q=80&w=800&auto=format&fit=crop"
            }
        };

        let currentQuestionIndex = 0;
        let scoreCounter = { 'A': 0, 'B': 0, 'C': 0, 'D': 0, 'E': 0 };

        function startQuiz() {
            document.getElementById('intro-screen').classList.remove('show-page');
            document.getElementById('intro-screen').classList.add('hide-page');
            
            document.getElementById('quiz-screen').classList.remove('hide-page');
            document.getElementById('quiz-screen').classList.add('show-page');
            
            currentQuestionIndex = 0;
            scoreCounter = { 'A': 0, 'B': 0, 'C': 0, 'D': 0, 'E': 0 };
            renderQuestion();
        }

        function renderQuestion() {
            const currentQuestion = quizData[currentQuestionIndex];
            
            // Update 3D Camera Focus dynamically based on actual chronological questions (1-5)
            update3DSceneForQuestion(currentQuestionIndex + 1);

            // Update UI elements
            document.getElementById('quiz-step-text').innerText = `QUESTION 0${currentQuestionIndex + 1}`;
            document.getElementById('quiz-progress-text').innerText = `${currentQuestionIndex + 1} / 5`;
            
            const progressPercent = ((currentQuestionIndex + 1) / 5) * 100;
            document.getElementById('progress-bar').style.width = `${progressPercent}%`;
            
            document.getElementById('question-text').innerText = currentQuestion.question;
            
            // Set text for options
            document.getElementById('opt-text-A').innerText = currentQuestion.options.A.text;
            document.getElementById('opt-text-B').innerText = currentQuestion.options.B.text;
            document.getElementById('opt-text-C').innerText = currentQuestion.options.C.text;
            document.getElementById('opt-text-D').innerText = currentQuestion.options.D.text;
            document.getElementById('opt-text-E').innerText = currentQuestion.options.E.text;
        }

        function selectOption(optKey) {
            const currentQuestion = quizData[currentQuestionIndex];
            const chosenStyle = currentQuestion.options[optKey].style;
            
            // Add score to the corresponding style
            scoreCounter[chosenStyle]++;

            // Smooth fade out & in logic for questions
            const quizContainer = document.getElementById('quiz-screen');
            quizContainer.style.opacity = '0.3';
            quizContainer.style.transform = 'translateY(10px)';

            setTimeout(() => {
                currentQuestionIndex++;
                if (currentQuestionIndex < quizData.length) {
                    renderQuestion();
                    quizContainer.style.opacity = '1';
                    quizContainer.style.transform = 'translateY(0)';
                } else {
                    showFinalResult();
                }
            }, 300);
        }

        function showFinalResult() {
            // Find the style with the highest score
            let maxScore = -1;
            let dominantStyle = 'A'; // Default to Hotel Style

            for (const [styleId, score] of Object.entries(scoreCounter)) {
                if (score > maxScore) {
                    maxScore = score;
                    dominantStyle = styleId;
                }
            }

            const metadata = styleMetadata[dominantStyle];

            // Update 3D colors and camera to perfect panoramic light blue aesthetic
            update3DSceneForFinalResult(dominantStyle);

            // Populate Result Panel
            document.getElementById('result-style-title').innerText = metadata.title;
            document.getElementById('result-style-desc').innerText = metadata.desc;
            document.getElementById('result-style-materials').innerText = metadata.materials;
            document.getElementById('result-promo-offer').innerHTML = `<i class="fa-solid fa-gift mr-2"></i> ${metadata.promo}`;
            document.getElementById('style-code').innerText = metadata.code;

            // Load high-quality real design photo with smooth transitions
            const styleImgElement = document.getElementById('style-image');
            styleImgElement.style.opacity = '0';
            setTimeout(() => {
                styleImgElement.src = metadata.image;
                styleImgElement.style.opacity = '1';
            }, 150);

            // Page Transition to Result View
            document.getElementById('quiz-screen').classList.remove('show-page');
            document.getElementById('quiz-screen').classList.add('hide-page');
            
            document.getElementById('result-screen').classList.remove('hide-page');
            document.getElementById('result-screen').classList.add('show-page');
        }

        function restartQuiz() {
            document.getElementById('result-screen').classList.remove('show-page');
            document.getElementById('result-screen').classList.add('hide-page');
            
            document.getElementById('intro-screen').classList.remove('hide-page');
            document.getElementById('intro-screen').classList.add('show-page');

            // Reset camera to cinematic initial view
            targetCameraPos = { x: 0, y: 3, z: 12 };
            targetLookAt = { x: 0, y: 1, z: 0 };
            lightSpot.color.setHex(0x3b82f6);
            lightSpot.intensity = 3;
        }

        function copyStyleCode() {
            const codeText = document.getElementById('style-code').innerText;
            
            // Frame safe fallback copy method
            const tempInput = document.createElement("input");
            tempInput.value = codeText;
            document.body.appendChild(tempInput);
            tempInput.select();
            document.execCommand("copy");
            document.body.removeChild(tempInput);

            // Play elegant feedback toast animation
            const toast = document.getElementById('toast-message');
            const copyIcon = document.getElementById('copy-icon');
            
            copyIcon.className = "fa-solid fa-check text-brandBlue-600";
            toast.style.opacity = '1';
            toast.style.transform = 'translateY(-10px) translateX(-50%)';

            setTimeout(() => {
                toast.style.opacity = '0';
                toast.style.transform = 'translateY(0) translateX(-50%)';
                copyIcon.className = "fa-regular fa-copy";
            }, 3000);
        }

        // Redirect to HouseStyle Official LINE with prefilled text template
        function redirectToLine() {
            const codeText = document.getElementById('style-code').innerText;
            const styleTitle = document.getElementById('result-style-title').innerText;
            
            // Construct a template targeting HouseStyle Bath
            const message = encodeURIComponent(`您好！我剛剛完成了好時代衛浴的「衛浴美學避難所」心理測驗，測出我最契合的專屬風格是：【${styleTitle}】！\n\n專屬優惠代碼：${codeText}\n\n我想預約免費門市諮詢與到府丈量，進一步規劃我的風格空間與乾濕分離配置！`);
            
            window.open(`https://line.me/R/msg/text/?${message}`, '_blank');
        }

        // --- STREAMING_CHUNK: Setting up the Three.js 3D Background Scene ---
        let scene, camera, renderer, lightSpot, ambientLight;
        let objects = {};
        let targetCameraPos = { x: 0, y: 3, z: 12 };
        let targetLookAt = { x: 0, y: 1, z: 0 };
        let currentLookAt = new THREE.Vector3(0, 1, 0);

        function init3D() {
            const container = document.getElementById('webgl-container');
            const width = window.innerWidth;
            const height = window.innerHeight;

            // Create Scene
            scene = new THREE.Scene();
            scene.background = new THREE.Color(0xf0f7ff);
            scene.fog = new THREE.FogExp2(0xf0f7ff, 0.05);

            // Create Camera
            camera = new THREE.PerspectiveCamera(45, width / height, 0.1, 100);
            camera.position.set(targetCameraPos.x, targetCameraPos.y, targetCameraPos.z);

            // Create Renderer
            renderer = new THREE.WebGLRenderer({ antialias: true, alpha: true });
            renderer.setSize(width, height);
            renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
            renderer.shadowMap.enabled = true;
            renderer.shadowMap.type = THREE.PCFSoftShadowMap;
            container.appendChild(renderer.domElement);

            // Create Ambient Light (Gentle soft overall lighting)
            ambientLight = new THREE.AmbientLight(0xffffff, 0.85);
            scene.add(ambientLight);

            // Create Spot Light for elegant focused highlight on products
            lightSpot = new THREE.SpotLight(0x3b82f6, 3, 20, Math.PI / 4, 0.5, 1);
            lightSpot.position.set(0, 6, 2);
            lightSpot.castShadow = true;
            scene.add(lightSpot);

            // Build a conceptual modern bathroom showroom setup
            buildShowroom();

            // Handle Resize
            window.addEventListener('resize', onWindowResize);

            // Start animation loop
            animate();
        }

        function buildShowroom() {
            const wallMaterial = new THREE.MeshStandardMaterial({ color: 0xffffff, roughness: 0.4 });
            const chromeMaterial = new THREE.MeshStandardMaterial({ color: 0xd1d5db, metalness: 0.9, roughness: 0.1 });
            const woodMaterial = new THREE.MeshStandardMaterial({ color: 0xcdb4db, roughness: 0.7 });
            const glassMaterial = new THREE.MeshPhysicalMaterial({ 
                color: 0xe0effe, 
                transparent: true, 
                opacity: 0.3, 
                roughness: 0.1,
                transmission: 0.9,
                thickness: 0.5
            });

            // 1. Backwall (Visual focus for Vanity setup)
            const wallGeo = new THREE.BoxGeometry(10, 5, 0.2);
            const wallMesh = new THREE.Mesh(wallGeo, wallMaterial);
            wallMesh.position.set(0, 2, -2);
            wallMesh.receiveShadow = true;
            scene.add(wallMesh);

            // 2. Tiled floor
            const floorGeo = new THREE.PlaneGeometry(20, 20);
            const floorMat = new THREE.MeshStandardMaterial({ color: 0xe2e8f0, roughness: 0.3 });
            const floorMesh = new THREE.Mesh(floorGeo, floorMat);
            floorMesh.rotation.x = -Math.PI / 2;
            floorMesh.receiveShadow = true;
            scene.add(floorMesh);

            // 3. Luxurious floating Vanity cabinet left
            const vanityCabinetGeo = new THREE.BoxGeometry(3, 0.6, 1.2);
            const vanityMesh = new THREE.Mesh(vanityCabinetGeo, woodMaterial);
            vanityMesh.position.set(-2, 1, -1.2);
            vanityMesh.castShadow = true;
            scene.add(vanityMesh);
            objects.vanity = vanityMesh;

            // 4. Mirror over Vanity
            const mirrorGeo = new THREE.CylinderGeometry(0.8, 0.8, 0.05, 32);
            const mirrorMesh = new THREE.Mesh(mirrorGeo, chromeMaterial);
            mirrorMesh.rotation.x = Math.PI / 2;
            mirrorMesh.position.set(-2, 2.2, -1.85);
            scene.add(mirrorMesh);
            objects.mirror = mirrorMesh;

            // 5. Classic Minimalist Oval Bathtub (Right side)
            const tubGroup = new THREE.Group();
            const tubOuterGeo = new THREE.CylinderGeometry(1.2, 1.0, 1.0, 32);
            const tubOuterMesh = new THREE.Mesh(tubOuterGeo, new THREE.MeshStandardMaterial({ color: 0xfcfdfe, roughness: 0.2 }));
            tubOuterMesh.castShadow = true;
            tubGroup.add(tubOuterMesh);
            
            tubGroup.position.set(2, 0.5, -0.5);
            scene.add(tubGroup);
            objects.tub = tubGroup;

            // 6. Premium Minimalist Glass Partition (Dry/Wet Separation representator)
            const glassFrameGeo = new THREE.BoxGeometry(0.1, 4, 1.8);
            const glassPanel = new THREE.Mesh(glassFrameGeo, glassMaterial);
            glassPanel.position.set(0.1, 2, -0.8);
            scene.add(glassPanel);
            objects.glassPanel = glassPanel;
        }

        function update3DSceneForQuestion(questionIndex) {
            switch(questionIndex) {
                case 1: // Q1: 放假怎麼過 -> Wide overview perspective
                    targetCameraPos = { x: 0, y: 3.2, z: 10 };
                    targetLookAt = { x: 0, y: 1.0, z: -1 };
                    lightSpot.color.setHex(0x3b82f6);
                    lightSpot.intensity = 3;
                    break;
                case 2: // Q2: 浴室最不能接受的情況 -> Zoom into Vanity/Mirror details
                    targetCameraPos = { x: -2.5, y: 2.0, z: 5 };
                    targetLookAt = { x: -2, y: 1.8, z: -1.5 };
                    lightSpot.color.setHex(0x2563eb);
                    lightSpot.intensity = 3.5;
                    break;
                case 3: // Q3: 重新裝潢浴室投資 -> Look down at cabinet & floor tiling
                    targetCameraPos = { x: -1.5, y: 0.8, z: 4.5 };
                    targetLookAt = { x: -2, y: 0.5, z: -1.2 };
                    lightSpot.color.setHex(0x1d4ed8);
                    lightSpot.intensity = 4;
                    break;
                case 4: // Q4: 每日踏進浴室第一感受 -> Transition towards Bathtub and Glass partition
                    targetCameraPos = { x: 1, y: 2.0, z: 6 };
                    targetLookAt = { x: 1.5, y: 1.2, z: -1 };
                    lightSpot.color.setHex(0x60a5fa);
                    lightSpot.intensity = 3.2;
                    break;
                case 5: // Q5: 符合生活態度的一句話 -> Complete panoramic zoom out
                    targetCameraPos = { x: 0, y: 3.5, z: 11 };
                    targetLookAt = { x: 0, y: 1.2, z: -0.5 };
                    lightSpot.color.setHex(0x38bdf8);
                    lightSpot.intensity = 3;
                    break;
                default:
                    targetCameraPos = { x: 0, y: 3, z: 12 };
                    targetLookAt = { x: 0, y: 1, z: 0 };
                    break;
            }
        }

        function update3DSceneForFinalResult(styleId) {
            targetCameraPos = { x: 0, y: 2.2, z: 7.5 };
            targetLookAt = { x: 0, y: 1.2, z: -1.5 };
            
            switch(styleId) {
                case 'A': // Hotel Elegant -> Luxurious Warm White 
                    lightSpot.color.setHex(0xfcd34d);
                    ambientLight.color.setHex(0xfffbeb);
                    lightSpot.intensity = 4;
                    break;
                case 'B': // Nordic Natural -> Clean daylight green-blue tone
                    lightSpot.color.setHex(0x86efac);
                    ambientLight.color.setHex(0xf0fdf4);
                    lightSpot.intensity = 3.5;
                    break;
                case 'C': // Modern Minimalist -> Slick cool blue
                    lightSpot.color.setHex(0x38bdf8);
                    ambientLight.color.setHex(0xf0f9ff);
                    lightSpot.intensity = 4.2;
                    break;
                case 'D': // Creamy Luxury -> Gentle warm sunset vibe
                    lightSpot.color.setHex(0xfde047);
                    ambientLight.color.setHex(0xfefce8);
                    lightSpot.intensity = 3.8;
                    break;
                case 'E': // Zen Muji -> Gentle cozy organic timber glow
                    lightSpot.color.setHex(0xfed7aa);
                    ambientLight.color.setHex(0xfffaf0);
                    lightSpot.intensity = 3.2;
                    break;
            }
        }

        function onWindowResize() {
            const width = window.innerWidth;
            const height = window.innerHeight;
            camera.aspect = width / height;
            camera.updateProjectionMatrix();
            renderer.setSize(width, height);
        }

        function animate() {
            requestAnimationFrame(animate);

            // Interpolate camera position for ultra slick transitions
            camera.position.x += (targetCameraPos.x - camera.position.x) * 0.05;
            camera.position.y += (targetCameraPos.y - camera.position.y) * 0.05;
            camera.position.z += (targetCameraPos.z - camera.position.z) * 0.05;

            // Interpolate camera target vector (LookAt)
            currentLookAt.x += (targetLookAt.x - currentLookAt.x) * 0.05;
            currentLookAt.y += (targetLookAt.y - currentLookAt.y) * 0.05;
            currentLookAt.z += (targetLookAt.z - currentLookAt.z) * 0.05;
            camera.lookAt(currentLookAt);

            // Subtle rotation of scene elements for ambient life
            if(objects.mirror) {
                objects.mirror.rotation.y += 0.002;
            }
            if(objects.tub) {
                objects.tub.rotation.y += 0.001;
            }

            renderer.render(scene, camera);
        }

        // Kickoff ThreeJS initialization inside window onload
        window.onload = function() {
            init3D();
        };
    </script>

<div id="tag-inspector-tooltip" style="display: none; left: 216px; top: 2px;">main</div></body></html>

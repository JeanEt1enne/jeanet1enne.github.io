<html
       <head>
    <title>Sorteio de Números</title>
    <style>
        /* Estilos... */
        @keyframes colorAnimation {
            0%, 100% { background-color: transparent; }
            50% { background-color: #ffcc00; }
        }
      body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
  body {
            width: 100vw;
            height: 100vh;
            background-image: url('./WhatsApp\ Image\ 2023-08-31\ at\ 13.46.33.jpeg');
           background-position: 100%;
            background-size:50% ;
            background-repeat: no-repeat;
                  }
 div.quadrado
             {
                 display: inline-block;
                 border: 2px solid black;
                 border-radius: 10px;
                background-color: lightblue;
                 width: 100%;
                  height: 200%;
                 background-image: url(./WhatsApp\ Image\ 2023-08-31\ at\ 13.46.33.jpeg);
                 background-size: 50%;
                background-repeat: repeat;
     }
          h1 {
            color: #333;
            margin-top: 20px;
        }
        button {
            background-color: #007bff;
            color: #fff;
            padding: 10px 20px;
            border: zoom-in;
            cursor: pointer;
            margin-block-start: 20px;
            margin-right: 600px;
        }
        button:hover {
            background-color: #0056b3;   
        }
        #sudoku {
            width: 100px;
            height: 300px;
            display: grid ;
            grid-template-columns: repeat(20, 100fr);
            grid-gap: 10px;
            margin: 20px auto;
            margin-left: 0;
            margin-right: 300;   
        }
        .numero {
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 18px;
            font-weight: bold;
            background-color: #eee;
            border: 2px solid #ddd;
            animation: colorAnimation 1.5s infinite;
            opacity: 0.7;
            transition: opacity 0.3s ease-in-out;
        }
        .numero.selected {
            opacity: 1;
        }
        .numero.sorteado {
            background-color: hsl(185, 100%, 50%);
            color: #ff0000;
            animation: colorAnimation  ;     
        }
        #resultado {
            margin-top: 250px;
            font-size: 18px;
            font-weight: bold;
            margin-right: 600px;
        }
    </style>
    <script>
        function sortearNumero() {
            const numeros = document.querySelectorAll('.numero');
            const numeroSorteado = Math.floor(Math.random() * numeros.length);
            const resultadoDiv = document.getElementById("resultado");
            numeros.forEach(n => n.classList.remove('selected', 'sorteado'));
            numeros[numeroSorteado].classList.add('selected', 'sorteado');
            resultadoDiv.innerHTML = 'Número sorteado: <span style="color:  #ff0000;">${numeros[numeroSorteado].textContent}</span>';
        }
    </script>
</head>
<body>
    <h1>Sorteio de Números</h1>
    <div id="sudoku">
         <!-- Cria os números de 1 a 25 no formato de Sudoku -->
         <div class="numero" onclick="selecionarNumero(this)">1</div>
         <div class="numero" onclick="selecionarNumero(this)">2</div>
         <div class="numero" onclick="selecionarNumero(this)">3</div>
         <div class="numero" onclick="selecionarNumero(this)">4</div>
         <div class="numero" onclick="selecionarNumero(this)">5</div>
         <div class="numero" onclick="selecionarNumero(this)">6</div>
         <div class="numero" onclick="selecionarNumero(this)">7</div>
         <div class="numero" onclick="selecionarNumero(this)">8</div>
         <div class="numero" onclick="selecionarNumero(this)">9</div>
         <div class="numero" onclick="selecionarNumero(this)">10</div>
         <div class="numero" onclick="selecionarNumero(this)">11</div>
         <div class="numero" onclick="selecionarNumero(this)">12</div>
         <div class="numero" onclick="selecionarNumero(this)">13</div>
         <div class="numero" onclick="selecionarNumero(this)">14</div>
         <div class="numero" onclick="selecionarNumero(this)">15</div>
         <div class="numero" onclick="selecionarNumero(this)">16</div>
         <div class="numero" onclick="selecionarNumero(this)">17</div>
         <div class="numero" onclick="selecionarNumero(this)">18</div>
         <div class="numero" onclick="selecionarNumero(this)">19</div>
         <div class="numero" onclick="selecionarNumero(this)">20</div>
         <div class="numero" onclick="selecionarNumero(this)">21</div>
         <div class="numero" onclick="selecionarNumero(this)">22</div>
         <div class="numero" onclick="selecionarNumero(this)">23</div>
         <div class="numero" onclick="selecionarNumero(this)">24</div>
         <div class="numero" onclick="selecionarNumero(this)">25</div>
         <div class="numero" onclick="selecionarNumero(this)">26</div>
         <div class="numero" onclick="selecionarNumero(this)">27</div>
         <div class="numero" onclick="selecionarNumero(this)">28</div>
         <div class="numero" onclick="selecionarNumero(this)">29</div>
         <div class="numero" onclick="selecionarNumero(this)">30</div>
         <div class="numero" onclick="selecionarNumero(this)">31</div>
         <div class="numero" onclick="selecionarNumero(this)">32</div>
         <div class="numero" onclick="selecionarNumero(this)">33</div>
         <div class="numero" onclick="selecionarNumero(this)">34</div>
         <div class="numero" onclick="selecionarNumero(this)">35</div>
         <div class="numero" onclick="selecionarNumero(this)">36</div>
         <div class="numero" onclick="selecionarNumero(this)">37</div>
         <div class="numero" onclick="selecionarNumero(this)">38</div>
         <div class="numero" onclick="selecionarNumero(this)">39</div>
         <div class="numero" onclick="selecionarNumero(this)">40</div>
         <div class="numero" onclick="selecionarNumero(this)">41</div>
         <div class="numero" onclick="selecionarNumero(this)">42</div>
         <div class="numero" onclick="selecionarNumero(this)">43</div>
         <div class="numero" onclick="selecionarNumero(this)">44</div>
         <div class="numero" onclick="selecionarNumero(this)">45</div>
         <div class="numero" onclick="selecionarNumero(this)">46</div>
         <div class="numero" onclick="selecionarNumero(this)">47</div>
         <div class="numero" onclick="selecionarNumero(this)">48</div>
         <div class="numero" onclick="selecionarNumero(this)">49</div>
         <div class="numero" onclick="selecionarNumero(this)">50</div>
         <div class="numero" onclick="selecionarNumero(this)">51</div>
         <div class="numero" onclick="selecionarNumero(this)">52</div>
         <div class="numero" onclick="selecionarNumero(this)">53</div>
         <div class="numero" onclick="selecionarNumero(this)">54</div>
         <div class="numero" onclick="selecionarNumero(this)">55</div>
         <div class="numero" onclick="selecionarNumero(this)">56</div>
         <div class="numero" onclick="selecionarNumero(this)">57</div>
         <div class="numero" onclick="selecionarNumero(this)">58</div>
         <div class="numero" onclick="selecionarNumero(this)">59</div>
         <div class="numero" onclick="selecionarNumero(this)">60</div>
         <div class="numero" onclick="selecionarNumero(this)">61</div>
         <div class="numero" onclick="selecionarNumero(this)">62</div>
         <div class="numero" onclick="selecionarNumero(this)">63</div>
         <div class="numero" onclick="selecionarNumero(this)">64</div>
         <div class="numero" onclick="selecionarNumero(this)">65</div>
         <div class="numero" onclick="selecionarNumero(this)">66</div>
         <div class="numero" onclick="selecionarNumero(this)">67</div>
         <div class="numero" onclick="selecionarNumero(this)">68</div>
         <div class="numero" onclick="selecionarNumero(this)">69</div>
         <div class="numero" onclick="selecionarNumero(this)">70</div>
         <div class="numero" onclick="selecionarNumero(this)">71</div>
         <div class="numero" onclick="selecionarNumero(this)">72</div>
         <div class="numero" onclick="selecionarNumero(this)">73</div>
         <div class="numero" onclick="selecionarNumero(this)">74</div>
         <div class="numero" onclick="selecionarNumero(this)">75</div>
         <div class="numero" onclick="selecionarNumero(this)">76</div>
         <div class="numero" onclick="selecionarNumero(this)">77</div>
         <div class="numero" onclick="selecionarNumero(this)">78</div>
         <div class="numero" onclick="selecionarNumero(this)">79</div>
         <div class="numero" onclick="selecionarNumero(this)">80</div>
         <div class="numero" onclick="selecionarNumero(this)">81</div>
         <div class="numero" onclick="selecionarNumero(this)">82</div>
         <div class="numero" onclick="selecionarNumero(this)">83</div>
         <div class="numero" onclick="selecionarNumero(this)">84</div>
         <div class="numero" onclick="selecionarNumero(this)">85</div>
         <div class="numero" onclick="selecionarNumero(this)">86</div>
         <div class="numero" onclick="selecionarNumero(this)">87</div>
         <div class="numero" onclick="selecionarNumero(this)">88</div>
         <div class="numero" onclick="selecionarNumero(this)">89</div>
         <div class="numero" onclick="selecionarNumero(this)">90</div>
         <div class="numero" onclick="selecionarNumero(this)">91</div>
         <div class="numero" onclick="selecionarNumero(this)">92</div>
         <div class="numero" onclick="selecionarNumero(this)">93</div>
         <div class="numero" onclick="selecionarNumero(this)">94</div>
         <div class="numero" onclick="selecionarNumero(this)">95</div>
         <div class="numero" onclick="selecionarNumero(this)">96</div>
         <div class="numero" onclick="selecionarNumero(this)">97</div>
         <div class="numero" onclick="selecionarNumero(this)">98</div>
         <div class="numero" onclick="selecionarNumero(this)">99</div>
         <div class="numero" onclick="selecionarNumero(this)">100</div>
         <div class="numero" onclick="selecionarNumero(this)">101</div>
         <div class="numero" onclick="selecionarNumero(this)">102</div>
         <div class="numero" onclick="selecionarNumero(this)">103</div>
         <div class="numero" onclick="selecionarNumero(this)">104</div>
         <div class="numero" onclick="selecionarNumero(this)">105</div>
         <div class="numero" onclick="selecionarNumero(this)">106</div>
         <div class="numero" onclick="selecionarNumero(this)">107</div>
         <div class="numero" onclick="selecionarNumero(this)">108</div>
         <div class="numero" onclick="selecionarNumero(this)">109</div>
         <div class="numero" onclick="selecionarNumero(this)">110</div>
         <div class="numero" onclick="selecionarNumero(this)">111</div>
         <div class="numero" onclick="selecionarNumero(this)">112</div>
         <div class="numero" onclick="selecionarNumero(this)">113</div>
         <div class="numero" onclick="selecionarNumero(this)">114</div>
         <div class="numero" onclick="selecionarNumero(this)">115</div>
         <div class="numero" onclick="selecionarNumero(this)">116</div>
         <div class="numero" onclick="selecionarNumero(this)">117</div>
         <div class="numero" onclick="selecionarNumero(this)">118</div>
         <div class="numero" onclick="selecionarNumero(this)">119</div>
         <div class="numero" onclick="selecionarNumero(this)">120</div>
         <div class="numero" onclick="selecionarNumero(this)">121</div>
         <div class="numero" onclick="selecionarNumero(this)">122</div>
         <div class="numero" onclick="selecionarNumero(this)">123</div>
         <div class="numero" onclick="selecionarNumero(this)">124</div>
         <div class="numero" onclick="selecionarNumero(this)">125</div>
         <div class="numero" onclick="selecionarNumero(this)">126</div>
         <div class="numero" onclick="selecionarNumero(this)">127</div>
         <div class="numero" onclick="selecionarNumero(this)">128</div>
         <div class="numero" onclick="selecionarNumero(this)">129</div>
         <div class="numero" onclick="selecionarNumero(this)">130</div>
         <div class="numero" onclick="selecionarNumero(this)">131</div>
         <div class="numero" onclick="selecionarNumero(this)">132</div>
         <div class="numero" onclick="selecionarNumero(this)">133</div>
         <div class="numero" onclick="selecionarNumero(this)">134</div>
         <div class="numero" onclick="selecionarNumero(this)">135</div>
         <div class="numero" onclick="selecionarNumero(this)">136</div>
         <div class="numero" onclick="selecionarNumero(this)">137</div>
         <div class="numero" onclick="selecionarNumero(this)">138</div>
         <div class="numero" onclick="selecionarNumero(this)">139</div>
         <div class="numero" onclick="selecionarNumero(this)">140</div>
         <div class="numero" onclick="selecionarNumero(this)">141</div>
         <div class="numero" onclick="selecionarNumero(this)">142</div>
         <div class="numero" onclick="selecionarNumero(this)">143</div>
         <div class="numero" onclick="selecionarNumero(this)">144</div>
         <div class="numero" onclick="selecionarNumero(this)">145</div>
         <div class="numero" onclick="selecionarNumero(this)">146</div>
         <div class="numero" onclick="selecionarNumero(this)">147</div>
         <div class="numero" onclick="selecionarNumero(this)">148</div>
         <div class="numero" onclick="selecionarNumero(this)">149</div>
         <div class="numero" onclick="selecionarNumero(this)">150</div>
         <div class="numero" onclick="selecionarNumero(this)">151</div>
         <div class="numero" onclick="selecionarNumero(this)">152</div>
         <div class="numero" onclick="selecionarNumero(this)">153</div>
         <div class="numero" onclick="selecionarNumero(this)">154</div>
         <div class="numero" onclick="selecionarNumero(this)">155</div>
         <div class="numero" onclick="selecionarNumero(this)">156</div>
         <div class="numero" onclick="selecionarNumero(this)">157</div>
         <div class="numero" onclick="selecionarNumero(this)">158</div>
         <div class="numero" onclick="selecionarNumero(this)">159</div>
         <div class="numero" onclick="selecionarNumero(this)">160</div>
         <div class="numero" onclick="selecionarNumero(this)">161</div>
         <div class="numero" onclick="selecionarNumero(this)">162</div>
         <div class="numero" onclick="selecionarNumero(this)">163</div>
         <div class="numero" onclick="selecionarNumero(this)">164</div>
         <div class="numero" onclick="selecionarNumero(this)">165</div>
         <div class="numero" onclick="selecionarNumero(this)">166</div>
         <div class="numero" onclick="selecionarNumero(this)">167</div>
         <div class="numero" onclick="selecionarNumero(this)">168</div>
         <div class="numero" onclick="selecionarNumero(this)">169</div>
         <div class="numero" onclick="selecionarNumero(this)">170</div>
         <div class="numero" onclick="selecionarNumero(this)">171</div>
         <div class="numero" onclick="selecionarNumero(this)">172</div>
         <div class="numero" onclick="selecionarNumero(this)">173</div>
         <div class="numero" onclick="selecionarNumero(this)">174</div>
         <div class="numero" onclick="selecionarNumero(this)">175</div>
         <div class="numero" onclick="selecionarNumero(this)">176</div>
         <div class="numero" onclick="selecionarNumero(this)">177</div>
         <div class="numero" onclick="selecionarNumero(this)">178</div>
         <div class="numero" onclick="selecionarNumero(this)">179</div>
         <div class="numero" onclick="selecionarNumero(this)">180</div>
         <div class="numero" onclick="selecionarNumero(this)">181</div>
         <div class="numero" onclick="selecionarNumero(this)">182</div>
         <div class="numero" onclick="selecionarNumero(this)">183</div>
         <div class="numero" onclick="selecionarNumero(this)">184</div>
         <div class="numero" onclick="selecionarNumero(this)">185</div>
         <div class="numero" onclick="selecionarNumero(this)">186</div>
         <div class="numero" onclick="selecionarNumero(this)">187</div>
         <div class="numero" onclick="selecionarNumero(this)">188</div>
         <div class="numero" onclick="selecionarNumero(this)">189</div>
         <div class="numero" onclick="selecionarNumero(this)">190</div>
         <div class="numero" onclick="selecionarNumero(this)">191</div>
         <div class="numero" onclick="selecionarNumero(this)">192</div>
         <div class="numero" onclick="selecionarNumero(this)">193</div>
         <div class="numero" onclick="selecionarNumero(this)">194</div>
         <div class="numero" onclick="selecionarNumero(this)">195</div>
         <div class="numero" onclick="selecionarNumero(this)">196</div>
         <div class="numero" onclick="selecionarNumero(this)">197</div>
         <div class="numero" onclick="selecionarNumero(this)">198</div>
         <div class="numero" onclick="selecionarNumero(this)">199</div>
         <div class="numero" onclick="selecionarNumero(this)">200</div>
         <div class="numero" onclick="selecionarNumero(this)">201</div>
         <div class="numero" onclick="selecionarNumero(this)">202</div>
         <div class="numero" onclick="selecionarNumero(this)">203</div>
         <div class="numero" onclick="selecionarNumero(this)">204</div>
         <div class="numero" onclick="selecionarNumero(this)">205</div>
         <div class="numero" onclick="selecionarNumero(this)">206</div>
         <div class="numero" onclick="selecionarNumero(this)">207</div>
         <div class="numero" onclick="selecionarNumero(this)">208</div>
         <div class="numero" onclick="selecionarNumero(this)">209</div>
         <div class="numero" onclick="selecionarNumero(this)">210</div>
         <div class="numero" onclick="selecionarNumero(this)">211</div>
         <div class="numero" onclick="selecionarNumero(this)">212</div>
         <div class="numero" onclick="selecionarNumero(this)">213</div>
         <div class="numero" onclick="selecionarNumero(this)">214</div>
         <div class="numero" onclick="selecionarNumero(this)">215</div>
         <div class="numero" onclick="selecionarNumero(this)">216</div>
         <div class="numero" onclick="selecionarNumero(this)">217</div>
         <div class="numero" onclick="selecionarNumero(this)">218</div>
         <div class="numero" onclick="selecionarNumero(this)">219</div>
         <div class="numero" onclick="selecionarNumero(this)">220</div>
         <div class="numero" onclick="selecionarNumero(this)">221</div>
         <div class="numero" onclick="selecionarNumero(this)">222</div>
         <div class="numero" onclick="selecionarNumero(this)">223</div>
         <div class="numero" onclick="selecionarNumero(this)">224</div>
         <div class="numero" onclick="selecionarNumero(this)">225</div>
         <div class="numero" onclick="selecionarNumero(this)">226</div>
         <div class="numero" onclick="selecionarNumero(this)">227</div>
         <div class="numero" onclick="selecionarNumero(this)">228</div>
         <div class="numero" onclick="selecionarNumero(this)">229</div>
         <div class="numero" onclick="selecionarNumero(this)">230</div>
         <div class="numero" onclick="selecionarNumero(this)">231</div>
         <div class="numero" onclick="selecionarNumero(this)">232</div>
         <div class="numero" onclick="selecionarNumero(this)">233</div>
         <div class="numero" onclick="selecionarNumero(this)">234</div>
         <div class="numero" onclick="selecionarNumero(this)">235</div>
         <div class="numero" onclick="selecionarNumero(this)">236</div>
         <div class="numero" onclick="selecionarNumero(this)">237</div>
         <div class="numero" onclick="selecionarNumero(this)">238</div>
         <div class="numero" onclick="selecionarNumero(this)">239</div>
         <div class="numero" onclick="selecionarNumero(this)">240</div>
         <div class="numero" onclick="selecionarNumero(this)">241</div>
         <div class="numero" onclick="selecionarNumero(this)">242</div>
         <div class="numero" onclick="selecionarNumero(this)">243</div>
         <div class="numero" onclick="selecionarNumero(this)">244</div>
         <div class="numero" onclick="selecionarNumero(this)">245</div>
         <div class="numero" onclick="selecionarNumero(this)">246</div>
         <div class="numero" onclick="selecionarNumero(this)">247</div>
         <div class="numero" onclick="selecionarNumero(this)">248</div>
         <div class="numero" onclick="selecionarNumero(this)">249</div>
         <div class="numero" onclick="selecionarNumero(this)">250</div>
         <div class="numero" onclick="selecionarNumero(this)">251</div>
         <div class="numero" onclick="selecionarNumero(this)">252</div>
         <div class="numero" onclick="selecionarNumero(this)">253</div>
         <div class="numero" onclick="selecionarNumero(this)">254</div>
         <div class="numero" onclick="selecionarNumero(this)">255</div>
         <div class="numero" onclick="selecionarNumero(this)">256</div>
         <div class="numero" onclick="selecionarNumero(this)">257</div>
         <div class="numero" onclick="selecionarNumero(this)">258</div>
         <div class="numero" onclick="selecionarNumero(this)">259</div>
         <div class="numero" onclick="selecionarNumero(this)">260</div>
         <div class="numero" onclick="selecionarNumero(this)">261</div>
         <div class="numero" onclick="selecionarNumero(this)">262</div>
         <div class="numero" onclick="selecionarNumero(this)">263</div>
         <div class="numero" onclick="selecionarNumero(this)">264</div>
         <div class="numero" onclick="selecionarNumero(this)">265</div>
         <div class="numero" onclick="selecionarNumero(this)">266</div>
         <div class="numero" onclick="selecionarNumero(this)">267</div>
         <div class="numero" onclick="selecionarNumero(this)">268</div>
         <div class="numero" onclick="selecionarNumero(this)">269</div>
         <div class="numero" onclick="selecionarNumero(this)">270</div>
         <div class="numero" onclick="selecionarNumero(this)">271</div>
         <div class="numero" onclick="selecionarNumero(this)">272</div>
         <div class="numero" onclick="selecionarNumero(this)">273</div>
         <div class="numero" onclick="selecionarNumero(this)">274</div>
         <div class="numero" onclick="selecionarNumero(this)">275</div>
         <div class="numero" onclick="selecionarNumero(this)">276</div>
         <div class="numero" onclick="selecionarNumero(this)">277</div>
         <div class="numero" onclick="selecionarNumero(this)">278</div>
         <div class="numero" onclick="selecionarNumero(this)">279</div>
         <div class="numero" onclick="selecionarNumero(this)">280</div>
         <div class="numero" onclick="selecionarNumero(this)">281</div>
         <div class="numero" onclick="selecionarNumero(this)">282</div>
         <div class="numero" onclick="selecionarNumero(this)">283</div>
         <div class="numero" onclick="selecionarNumero(this)">284</div>
         <div class="numero" onclick="selecionarNumero(this)">285</div>
         <div class="numero" onclick="selecionarNumero(this)">286</div>
         <div class="numero" onclick="selecionarNumero(this)">287</div>
         <div class="numero" onclick="selecionarNumero(this)">288</div>
         <div class="numero" onclick="selecionarNumero(this)">289</div>
         <div class="numero" onclick="selecionarNumero(this)">290</div>
         <div class="numero" onclick="selecionarNumero(this)">291</div>
         <div class="numero" onclick="selecionarNumero(this)">292</div>
         <div class="numero" onclick="selecionarNumero(this)">293</div>
         <div class="numero" onclick="selecionarNumero(this)">294</div>
         <div class="numero" onclick="selecionarNumero(this)">295</div>
         <div class="numero" onclick="selecionarNumero(this)">296</div>
         <div class="numero" onclick="selecionarNumero(this)">297</div>
         <div class="numero" onclick="selecionarNumero(this)">298</div>
         <div class="numero" onclick="selecionarNumero(this)">299</div>
         <div class="numero" onclick="selecionarNumero(this)">300</div>   
    </div>
    <div id="resultado"></div>
    <button onclick="sortearNumero()">Sortear Número</button> 
<div class='quadrado'></div>

</body>
</html>

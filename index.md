# Masked Generative Model-Based Target Speaker Extraction Method by Leveraging Discrete Acoustic Tokens

## Abstract

Most existing target speaker extraction (TSE) methods rely on a discriminative approach, which often leads to unpleasant distortions and limited generalization ability. In contrast, the generative approach has recently shown promising results in producing high-quality signals. In this paper, we propose a novel TSE method based on the masked generative model that leverages discrete acoustic tokens. During training, the target speaker’s speech is encoded with a neural codec to derive acoustic tokens, which are then partially masked. The model is optimized to predict these masked tokens by using tokens from both the mixed signal and the target speaker’s enrollment, with the help of attention mechanism. During inference, multiple iterations are performed, progressing from fully masked tokens to fully predicted ones. Tokens with high confidence are preserved, allowing to gradually predict more accurate tokens. Experiments show that the proposed method is effective in performing extraction.

<p></p>

## Audio Demos

<!-- Source: M1 -->
<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>


<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>


<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>


<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>


<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>


<div class="row">
    <div class="col-12 ml-auto">
          <!-- M1 to M -->
            <table width="400">
                <tr>
                    <td style="width: 25%">mix</td>
                    <td style="width: 25%">clean s1</td>
                    <td style="width: 25%">enroll s1</td>
                    <td style="width: 25%">extract s1</td>
                </tr>
                <tr>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>clean s2</td>
                    <td>enroll s2</td>
                    <td>extract s2</td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extract_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </table>
    </div>
</div>

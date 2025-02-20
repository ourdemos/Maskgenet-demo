# Masked Generative Model-Based Target Speaker extractedion Method by Leveraging Discrete Acoustic Tokens

## Abstract

Most existing target speaker extractedion (TSE) methods rely on a discriminative approach, which often leads to unpleasant distortions and limited generalization ability. In contrast, the generative approach has recently shown promising results in producing high-quality signals. In this paper, we propose a novel TSE method based on the masked generative model that leverages discrete acoustic tokens. During training, the target speaker’s speech is encoded with a neural codec to derive acoustic tokens, which are then partially masked. The model is optimized to predict these masked tokens by using tokens from both the mixed signal and the target speaker’s enrollment, with the help of attention mechanism. During inference, multiple iterations are performed, progressing from fully masked tokens to fully predicted ones. Tokens with high confidence are preserved, allowing to gradually predict more accurate tokens. Experiments show that the proposed method is effective in performing extractedion.

<p></p>

## Audio Demos

<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmoke; display: table;">
            <thead>
                <tr>
                    <th style="width: 25%;">Mix</th>
                    <th style="width: 25%;">Clean</th>
                    <th style="width: 25%;">Enroll</th>
                    <th style="width: 25%;">Extracted</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td rowspan="4">
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td rowspan="4">
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td rowspan="4">
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td rowspan="4">
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td></td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/1188-133604-0022_1221-135767-0019.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/5639-40744-0034_4507-16021-0058.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/6829-68769-0026_1284-1180-0030.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/8230-279154-0017_8224-274384-0004.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <!---next---->
                <tr>
                    <td>
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/8455-210777-0020_61-70968-0054.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <!---next--->
                <tr>
                    <td>
                        <p>Mix</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/mix/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S1 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s1/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
                <tr>
                    <td>
                    </td>
                    <td>
                        <p>S2 clean</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/clean_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 enroll</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/enroll_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                    <td>
                        <p>S2 extracted</p>
                        <audio id="player" controls style="width: 100%;">
                            <source src="audio/extracted_s2/8463-294828-0009_3570-5694-0015.wav" type="audio/wav" />
                        </audio>
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</div>

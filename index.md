# Masked Generative Model-Based Target Speaker extractedion Method by Leveraging Discrete Acoustic Tokens

## Abstract

Most existing target speaker extractedion (TSE) methods rely on a discriminative approach, which often leads to unpleasant distortions and limited generalization ability. In contrast, the generative approach has recently shown promising results in producing high-quality signals. In this paper, we propose a novel TSE method based on the masked generative model that leverages discrete acoustic tokens. During training, the target speaker’s speech is encoded with a neural codec to derive acoustic tokens, which are then partially masked. The model is optimized to predict these masked tokens by using tokens from both the mixed signal and the target speaker’s enrollment, with the help of attention mechanism. During inference, multiple iterations are performed, progressing from fully masked tokens to fully predicted ones. Tokens with high confidence are preserved, allowing to gradually predict more accurate tokens. Experiments show that the proposed method is effective in performing extractedion.

<p></p>

## Audio Demos

<div class="row">
    <div class="col-12 ml-auto">
        <table class="table table-responsive align-content-left" style="background-color: whitesmake; display: table;">
            <thead>
                <tr>
                    <th style="width: 14%;">Mix</th>
                    <th style="width: 14%;">Enroll</th>
                    <th style="width: 14%;">Target</th>
                    <th style="width: 14%;">MaskGENet (Ours)</th>
                    <th style="width: 14%;">CIENet256</th>
                    <th style="width: 14%;">SpEx+</th>
                    </tr>
            </thead>
		<tbody>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/FF/5142-33396-0018_2094-142345-0043/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MF/7127-75947-0040_237-126133-0002/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/7729-102255-0023_61-70968-0033/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Clean/MM/8455-210777-0058_7176-88083-0006/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/FF/3729-6852-0038_8463-294828-0003/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4446-2275-0008_2300-131720-0032/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MF/4992-23283-0018_1188-133604-0013/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
            <tr>
                <td>
                    <p>Mix</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/Mixture.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Enroll</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/Enroll1.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>Target</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/S1_Clean.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>MaskGENet (Ours)</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/S1_MaskGENet.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>CIENet256</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/S1_CIENet256.wav" type="audio/wav" />
                        </audio>
                </td>
                <td>
                    <p>SpEx+</p>
                    
                        <audio controls style="width: 100%;">
                            <source src="audio/Libri2Mix-Noisy/MM/7729-102255-0017_672-122797-0063/S1_SpEx+.wav" type="audio/wav" />
                        </audio>
                </td>
            </tr>
		</tbody>
		</table>
    </div>
</div>

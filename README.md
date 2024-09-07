A Table for a systematic review of UNet-Like change detection. For the complete article, please refer to 
C. Wu, L. Zhang, B. Du et al., “UNet-Like Remote Sensing Change Detection: A review of current models and research directions,” IEEE Geoscience and Remote Sensing Magazine, pp. 2-31, 2024. (https://ieeexplore.ieee.org/abstract/document/10616141)

#### APPENDIX TABLE I SYSTEMATIC REVIEW OF UNET-LIKE CHANGE DETECTION MODELS CORRESPONDING TO DIFFRENT BLOCKS
|  | Name | Year | Encoder Structure | Symmetry | Encoder module | Feature to Decoder | Skip-connection | Data fusion | Loss |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | FC-EF[1] | 2018 | EF | Sym | Conv | EF | S-C | EF | CE |
| 2 | FC-Siam-Conc[1] | 2018 | Siam | Sym | Conv | T1 | S-C | Conc | CE |
| 3 | FC-Siam-Diff[1] | 2018 | Siam | Sym | Conv | T1 | S-C | Dif | CE |
| 4 | Jaturapitpornchai, et al. [2] | 2019 | EF | Sym | Conv | EF | S-C | EF | wBCE |
| 5 | FCN-PP[3] | 2019 | EF + **Diff** + **Multivariate morphological reconstruction (MMR)** | Sym | Conv | EF + **Pyramid pooling (PP)** | S-C | EF | wCE |
| 6 | Peng, et al. [4] | 2019 | EF | Sym | Res | EF | **UNet++** | EF | wBCE + Dice |
| 7 | CDGAN[5] | 2020 | Siam | Sym | Conv | Conc | S-C | Conc | **GAN** |
| 8 | PGA-SiamNet[6] | 2020 | Siam | Sym | **ASPP** | **Co-attention** | S-C | **Change residual process** | BCE |
| 9 | Liu, et al. [7] | 2020 | EF | Sym | **Depthwise separable conv** | EF | S-C | EF | BCE + Dice |
| 10 | DTCDSCN[8] | 2020 | Siam | Sym | **Squeeze and excitation block (SE Block)** | Dif + **Spatial pyramid pooling module** | S-C | Dif | wBCE + **Change detection loss (CDL)** + **Deep supervision** + **Multitask** |
| 11 | Peng, et al. [9] | 2020 | EF | Sym | Res | EF | **Attention** + **UNet++** | EF | wBCE + **GAN (Segmentation adversarial loss + Entropy adversarial loss)** |
| 12 | DDCNN[10] | 2020 | EF | Sym | Res | EF | **UNet++** | EF + **Difference enhancement** | BCE |
| 13 | Sun, et al. [11] | 2020 | EF | Sym | Conv | EF | S-C | EF | **Multi-task** |
| 14 | IFN[12] | 2020 | Siam | Sym | Conv | Conc | S-C | Conc | BCE + Dice + **Deep supervision** |
| 15 | Yang, et al. [13] | 2021 | Siam | Sym | Res | Conc + **High-Level feature fusion block (HFFB)** | S-C | Conc + **Fusion block (FB)** | CE |
| 16 | HDFNet[14] | 2021 | Siam | Sym | Conv | **Fusion Steam** + Conv | S-C | Conc | Focal + **Multilevel supervision** |
| 17 | Adriano, et al. [15] | 2021 | Pseudo-Siam | Sym | Conv | Conc + **Attention gate** | S-C | Conc + **Attention gate** | CE |
| 18 | DSA-Net[16] | 2021 | Siam | Sym | Strided conv + **Attention guided cross-layer addition (ACLA)** | Conc + **ASPP** | S-C | Conc + **Spatial attention mechanism (SAM)** | **Deep supervision** + BCD |
| 19 | SNUNet-CD[17] | 2021 | Siam | Sym | Res | T1 | **UNet++** | Conc | **Ensemble channel attention module (ECAM)** + wCE +Dice |
| 20 | MSPSNet[18] | 2021 | Siam | Sym | Res | Conc + **Parallel convolutional structure (PCS)** | S-C | Conc + **Parallel convolutional structure (PCS)** | wCE + Dice |
| 21 | MASNet[19] | 2021 | Siam | Sym | **Selective kernel convolution (SKConv)** | Conc + **Attention feature fusion module (AFFM)** | S-C | Conc + **Attention feature fusion module (AFFM)** | BCE |
| 22 | DP-CD-Net[20] | 2021 | Pseduo-Siam | Sym | Res | Diff | S-C + Decoder S-C | Diff | CE + **Auxiliary loss (AUX loss)** |
| 23 | DTCDN[21] | 2021 | EF + Translation | Sym | **Depthwise & pointwise Conv** | EF | **UNet++** | EF | Weighted Focal + **Deep supervision** |
| 24 | Li, et al. [22] | 2021 | EF | Sym | Conv + **ASPP** | EF | S-C | Conc | wBCE + Dice |
| 25 | DCFF-Net[23] | 2021 | EF + Siam | Sym | Conv | EF | **UNet++** | Conc + **Multi-features fusion (FF) module** | BCE + **Self-adjusting dice loss (SADICE)** |
| 26 | Multitask L-Unet[24] | 2021 | **Time-series input** + Siam | Sym | Conv | **Long short-term memory (LSTM)** | S-C | **Long short-term memory (LSTM)** | CE + **Multi-task**  |
| 27 | SCDNET[25] | 2021 | Siam | Sym | Res | T1/T2 + **Multi-scale atrous convolution (MAC)** | S-C | Diff + **Attention** | CE + **Deep Fusion** |
| 28 | ADS-Net[26] | 2021 | Siam | non-Sym | Conv | Dif + Conc + **Attention** | **Weighted sum** | Diff + Conc + **Attention**  | **Deep supervision** + Focal |
| 29 | BASNet[27] | 2021 | Siam | Sym | Res | Conc + **Multiscale-paired fusion module (MPFM)** + **Spatial pyramid pooling module (SPPM)** | S-C + **Guiding flows** + **Max pooling** | Conc + **Multiscale-paired fusion module (MPFM)** | BCE + **Multi-level feature aggregation + Structural similarity (SSIM)** |
| 30 | DCA-Net[28] | 2021 | Siam | Sym | Res | **Dual correlation attention module (DCAM)** | S-C | **Dual correlation attention module (DCAM)** | **Bounding box regression loss** + **Change confidence prediction loss** |
| 31 | DifUnet++[29] | 2021 | Siam + EF | Sym | Conv | Dif + Conc | **UNet++** | Dif + Conc | Focal |
| 32 | CLNet[30] | 2021 | EF | Sym | **Cross layer blocks (CLB)** | EF | S-C | EF | wBCE + Dice |
| 33 | Siam-GL[31] | 2021 | Siam | Sym | Conv | Conc + **Binary change mask** | S-C | Conc | **Weighted softmax** + **Multi-class change detection** |
| 34 | CS-HSNet[32] | 2021 | Siam | non-Sym | **Cross-Siamese Res2Net (CSRes2Net) module** | **Hierarchical-split attention block** + Conc | Conc | **Hierarchical-split attention block** + Conc | nan |
| 35 | EGRCNN[33] | 2022 | Siam | Sym | Conv | **Difference analysis** | S-C | **Difference analysis** | Focal + **Deep supervision** + **Edge constraint** |
| 36 | UCDNet[34] | 2022 | Siam | Sym | Conv + **Modified residual connection** | Conc | S-C | Conc + **New spatial pyramid pooling (NSPP) block** | wCE + **modified kappa loss** |
| 37 | FCCDN[35] | 2022 | Siam | Sym | **Squeeze and excitation ResNet (SE-ResNet)** | **Nonlocal feature pyramid network (NL-FPN)** + **Dense fusion (DFM)** | S-C | **Dense fusion (DFM)** | **Self-supervised learning** + **Multi-task** + BCE + Dice |
| 38 | Siamese_AUNet[36] | 2022 | Siam | Sym | Conv + **Feature attention model (FAM)** | **ASPP** + Conc | S-C | Conc | BCE |
| 39 | ISNet[37] | 2022 | Siam | Sym | Res + **Channel attention (CA)** | **Margin maximization (MM)** + **Spatial attention (SA)** | S-C | **Margin maximization (MM)** + **Spatial attention (SA)** | Dice + CE |
| 40 | MCDnet [38] | 2022 | Siam | Sym | Conv + **Bidirectional feature pyramid network (BiFPN)**  | **Change feature fusion module (CFFM)** | S-C | **Change feature fusion module (CFFM)** | **Multi-task** + **Change contrast loss (CCL)** |
| 41 | LWCDNet[39] | 2022 | EF | Sym | **Artificial padding convolution (APC)**  | EF + **Convolutional block attention module (CBAM)** | S-C | EF | wCE + **Lovász** |
| 42 | ForkNet[40] | 2022 | Siam | Sym | Conv + **Cross-resolution attention module (CRAM)** + **Feature pyramid network (FPN)** | Diff | S-C + **Feature pyramid network (FPN)** | Diff | **Pyramid Tversky loss** + Focal |
| 43 | Forest-CD[41] | 2022 | Siam | Sym | **Transformer** | Conc + **Pyramid pooling module (PPM)** | S-C | Conc | **Multi-layer stacking** + **OCR** + **Deep supervision** + Focal + Dice |
| 44 | LGSAA-Net[42] | 2022 | Siam + **Diff Image** | Sym | Conv | Diff + Conc + **Scale-adaptive attention (SAA)** + **Multilayer perceptron based on patches embedding (MLPPE)** | S-C | Diff + Conc + **Scale-adaptive attention (SAA)** + **Multilayer perceptron based on patches embedding (MLPPE)** | nan |
| 45 | DARNet[43] | 2022 | Siam | Sym | Conv | **Hybrid attention module (HAM)** | **Densely Connected** | **Hybrid attention module (HAM)** | **Deep supervision** + BCE + Dice |
| 46 | EUNet[44] | 2022 | Siam | Sym | **Encoder with efficient convolution module (EECM)** | **Fusion operation (FO)** | UNet++ | **Fusion operation (FO)**  | **Multi-layer** + wCE + Dice |
| 47 | FCDNet[45] | 2022 | Siam | Sym | **Depthwise over-parameterized convolutional layer (DOConv)** | Diff + **Multireceptive field position enhancement module (MRPEM)** | **Densely Connected** | Diff + **Multireceptive field position enhancement module (MRPEM)** | wCE + Dice |
| 48 | SwinSUNet[46] | 2022 | Siam | Sym | **Swin Transformer** | Conc + **Swin Transformer** | S-C | Conc | nan |
| 49 | EGDE-Net[47] | 2022 | Siam | Sym | **Edge-guided Transformer blocks (EGTB）** | Dif + **Feature differential enhancement modules (FDEM)** | S-C | Dif + **Feature differential enhancement modules (FDEM)** | BCE + **Edge loss** |
| 50 | SMD-Net[48] | 2022 | Siam | Sym | Res | Conc + **Siamese residual multi-kernel pooling module (SRMP)** | S-C | Conc + **Feature difference module (FDM)** | BCE + **Tversky** |
| 51 | SSANet[49] | 2022 | EF + **Dif** | Sym | **Multicore channel-aligning attention (MCA) module** + **Feature differential reconfiguration (FDR) module** | EF + Addition | S-C | EF + Addition | **Batch balance contrast loss** |
| 52 | DESSN[50] | 2022 | Siam | Sym | **Asymmetric double convolution with Ghost (ADCG)** + **Difference enhancement (DE) module** | Conc + **Spatial–spectral nonlocal (SSN) module** | S-C | **Difference enhancement (DE) module** | BCE |
| 53 | TransUNetCD [51] | 2022 | Siam | Sym | Conv | **Embedding** + **Transformer** | S-C | Conc | **Difference enhance** + Dice |
| 54 | Lv, et al. [52] | 2022 | Siam + **Dif** | Sym | Conv + **Convolutional block attention module (CBAM)** | **Multiscale dilation convolution module (MDCM)** | S-C | Conc | BCE |
| 55 | FHD[53] | 2022 | Siam | Sym | **Mix Transformer (MiT)** | **Time-specific feature (TSF)** + **Hierarchical differentiation (HD) modules** | S-C | **Time-specific feature (TSF)** + **Hierarchical differentiation (HD) modules** | CE |
| 56 | DPCC-Net[54] | 2022 | Siam | non-Sym | Conv | **Dual-perspective fusion (DPF)** | Conc | **Dual-perspective fusion (DPF)** | **Tanimoto** |
| 57 | CDENet[55] | 2022 | Siam | Sym | Conv | **Transformer** + **Content difference enhancement module (CDEM)** | S-C | **Content difference enhancement module (CDEM)** | BCE + Dice |
| 58 | HMCNet[56] | 2022 | Siam | Sym | Res | **Multilayer perceptron (MLP)** | S-C | Conc | wCE + Dice |
| 59 | STransUNet[57] | 2022 | Siam | Sym | Conv | **Transformer** + **Cross-enhanced adaptive fusion (CEAF)** | S-C | **Cross-enhanced adaptive fusion (CEAF)** | nan |
| 60 | DA-MSCDNet[58] | 2022 | Siam | Sym | Conv | **Domain adaptation-based feature constraints** + Dif | S-C | Dif | **MK-MMD** + **Multi-layer stacking** + BCE + Dice |
| 61 | HFA-Net[59] | 2022 | Siam | Sym | **High frequency attention block (HFAB)** | Conc | S-C | Conc | BCE |
| 62 | Li, et al. [60] | 2022 | Siam | non-Sym | Res | **Temporal feature interaction module (TFIM)** | **Guided refinement module (GRM)** | **Temporal feature interaction module (TFIM)** | BCE + Dice |
| 63 | SFCCD[61] | 2022 | Siam | Sym | Res | **Multiscale feature fusion module (MSFF)** | S-C | **Global channel attention module (GCA)** + **Multiscale feature fusion module (MSFF)** | **Multi-task** + BCE |
| 64 | PCFN[62] | 2022 | Siam | Sym | Res | Conc | S-C | Conc | **Multi-task** + **Feature difference enhancement** + wCE |
| 65 | DAFT[63] | 2023 | Siam | Sym | **AFFormer** | **Multilayer Conc** | S-C | **Differential features enhancement module (DFEM)** | BCE + **Deep supervision** |
| 66 | AMIO-Net[64] | 2023 | Siam | Sym | Conv + **Multi-scale deep features** | **Pyramid Pooling Attention Module (PPAM)** + Conc | S-C | Conc | CE + Dice |
| 67 | AFDE-Net[65] | 2023 | Siam | Sym | Conv | Dif | S-C | Dif + **Ensemble spatial-channel attention fusion (ESCAF) module** | wCE + **Deep supervision** |
| 68 | AFNUNET[66]  | 2023 | EF | Sym | Res | EF | **UNet++** | EF | **Multi-layer features** + **Adaptive fusion module (AFM)** + BCE + **Bray-curtis ordination** |
| 69 | ConvTransNet[67] | 2023 | Siam | Sym | **CNN-Transformer** | Conc | S-C | Conc | wCE |
| 70 | A2Net[68] | 2023 | Siam | Sym | Res | **Neighbor aggregation module (NAM)** + Dif + **Progressive change identifying module (PCIM)** | S-C | **Neighbor aggregation module (NAM)** + Dif + **Progressive change identifying module (PCIM)** | BCE + Dice + **Deep supervision** |
| 71 | Lv, et al. [69] | 2023 | Siam | Sym | Conv | Conc + **Position channel attention module (PCAM)** | S-C | Conc + **Multiscale information attention module (MIAM)** | **Change gradient guided module** + CE |
| 72 | WNet[70] | 2023 | Siam | Sym | **Deformable Residual (D-Res)** + **Swin-Transformer** | Dif + Conc + **CNN–Transformer fusion module (CTFM)** | S-C | Dif + Conc + **CNN–Transformer fusion module (CTFM)** | CE + Dice |
| 73 | SSCFNet[71] | 2023 | Siam | non-Sym | Res | Dif + **Spatial-spectral cross fusion module** | Add | Dif + **Spatial-spectral cross fusion module** | BCE + **Deep supervision** |
| 74 | TCIANet[72] | 2023 | Siam | non-Sym | Res | **Filter-based visual tokenizer (FVT)** + **Progressive sampling vision (PSM)** + **Transformer** + Dif | Conc | **Feature fusion module (FFM)** + **Contour-graph reasoning module (CGRM)** + Dif | CE |
| 75 | HSSENet[73] | 2023 | Siam | Sym | Conv + **Transformer** | Conc + **Spatiotemporal enhancement module (STEM)** | S-C | Dif | **Deep supervision** + CE |
| 76 | SAGNet[74] | 2023 | Siam | non-Sym | Res | **Global semantic aggregation module (GSAM)** | Add | Dif + **Cross-scale fusion module (CFM)** + Conc + **Bilateral feature fusion module (BFEM)** | BCE |
| 77 | DMINet[75] | 2023 | Siam | non-Sym | Conv | **Joint attention module** + Dif + Conc | **Incremental aggregation** | **Joint attention module** +Dif + Conc | CE + **Deep supervision** |
| 78 | DGANet[76] | 2023 | Siam | non-Sym | Conv | **Difference-guided aggregation module (DGAM)** | Conc | **Weighted metric module (WMM)** | **Batch-balanced contrastive loss (BCL)** + **Change magnitude contrastive loss (CMCL)** |
| 79 | ACAHNet[77] | 2023 | Siam | Sym | Conv | Conc+ **Semantic Generation** + **Asymmetric multihead crossover attention (AMCA)** | S-C | Conc + **Three branch aggregation (TBA)** | wCE + Dice |
| 80 | FMCD[78] | 2023 | Siam | Sym | **EfficientNet** | **Multilevel feature interaction module** + **Mix block** | S-C | **Mix attention block (MAB)** | BCE + **Domain adaption loss** |
| 81 | TSNet[79] | 2023 | Siam + **Conc** | Sym | **EfficientNet** | **ConvGRU** + **Dual channel attention module** | S-C | **ConvGRU** + **Dual channel attention module** | BCE + Dice |
| 82 | MFSNet[80] | 2023 | Siam | Sym | Conv | Conc | **UNet++** | Conc | **Deep supervision** + BCE + Dice |
| 83 | HANet[81] | 2023 | Siam | Sym | Conv | **Hierarchical Attention Network (HAN)** | S-C | **Hierarchical Attention Network (HAN)** | wCE + Dice |
| 84 | T-Unet[82] | 2023 | Siam + **Dif** | Sym | Conv + **Multi-branch spatial-spectral cross attention (MBSSCA) module** | **Multi-branch spatial-spectral cross attention (MBSSCA) module** | S-C | **Multi-branch spatial-spectral cross attention (MBSSCA) module** | BCE + Dice |
| 85 | CGNet[83] | 2023 | Siam | Sym | Conv | Conc + **Change guide module (CGM)** | S-C | Conc + **Change guide module (CGM)** | CE + **Deep supervision** |
| 86 | SAAN[84] | 2023 | Siam | Sym | **EfficientNet** | Conc | S-C | **Similarity-guided attention flow module** | BCE + Dice + **Deep supervision** + **Contrastive loss** |

*In the table, the abbreviations are explained as: early fusion (EF), Siamese structure (Siam), pseudo-Siamese structure (pseudo-Siam), symmetry (Sym), non-symmetry (Non-sym), convolution module (Conv), residual module (Res) module, concatenation (Conc), difference (Dif), features from one time (T1/T2), and skip-connection (S-C). These abbreviations mostly indicate the basic blocks for UNet-like change detection models.

#### REFERENCES
[1]	R. C. Daudt, B. L. Saux, and A. Boulch, “Fully Convolutional Siamese Networks for Change Detection,” in 2018 25th IEEE International Conference on Image Processing (ICIP), 2018, pp. 4063-4067.

[2]	R. Jaturapitpornchai, M. Matsuoka, N. Kanemoto, S. Kuzuoka, R. Ito, and R. Nakamura, “Newly Built Construction Detection in SAR Images Using Deep Learning,” Remote Sensing, vol. 11, no. 12, 2019.

[3]	T. Lei, Y. Zhang, Z. Lv, S. Li, S. Liu, and A. K. Nandi, “Landslide Inventory Mapping From Bitemporal Images Using Deep Convolutional Neural Networks,” IEEE Geoscience and Remote Sensing Letters, vol. 16, no. 6, pp. 982-986, 2019.

[4]	D. Peng, Y. Zhang, and H. Guan, “End-to-End Change Detection for High Resolution Satellite Images Using Improved UNet++,” Remote Sensing, vol. 11, no. 11, p. 1382, 2019.

[5]	B. Hou, Q. Liu, H. Wang, and Y. Wang, “From W-Net to CDGAN: Bitemporal Change Detection via Deep Learning Techniques,” IEEE Transactions on Geoscience and Remote Sensing, vol. 58, no. 3, pp. 1790-1802, 2020.

[6]	H. Jiang, X. Hu, K. Li, J. Zhang, J. Gong, and M. Zhang, “PGA-SiamNet: Pyramid Feature-Based Attention-Guided Siamese Network for Remote Sensing Orthoimagery Building Change Detection,” Remote Sensing, vol. 12, no. 3, 2020.

[7]	R. Liu, D. Jiang, L. Zhang, and Z. Zhang, “Deep Depthwise Separable Convolutional Network for Change Detection in Optical Aerial Images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 13, pp. 1109-1118, 2020.

[8]	Y. Liu, C. Pang, Z. Zhan, X. Zhang, and X. Yang, “Building Change Detection for Remote Sensing Images Using a Dual-Task Constrained Deep Siamese Convolutional Network Model,” IEEE Geoscience and Remote Sensing Letters, vol. 18, no. 5, pp. 811-815, 2021.

[9]	D. Peng, L. Bruzzone, Y. Zhang, H. Guan, H. Ding, and X. Huang, “SemiCDNet: A Semisupervised Convolutional Neural Network for Change Detection in High Resolution Remote-Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 59, no. 7, pp. 5891-5906, 2021.

[10]	X. Peng, R. Zhong, Z. Li, and Q. Li, “Optical Remote Sensing Image Change Detection Based on Attention Mechanism and Image Difference,” IEEE Transactions on Geoscience and Remote Sensing, vol. 59, no. 9, pp. 7296-7307, 2021.

[11]	Y. Sun, X. Zhang, J. Huang, H. Wang, and Q. Xin, “Fine-Grained Building Change Detection From Very High-Spatial-Resolution Remote Sensing Images Based on Deep Multitask Learning,” IEEE Geoscience and Remote Sensing Letters, pp. 1-5, 2020.

[12]	C. Zhang et al., “A deeply supervised image fusion network for change detection in high resolution bi-temporal remote sensing images,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 166, pp. 183-200, 2020/08/01/ 2020.

[13]	L. Yang, Y. Chen, S. Song, F. Li, and G. Huang, “Deep Siamese Networks Based Change Detection with Remote Sensing Images,” Remote Sensing, vol. 13, no. 17, p. 3394, 2021.

[14]	Y. Zhang, L. Fu, Y. Li, and Y. Zhang, “HDFNet: Hierarchical Dynamic Fusion Network for Change Detection in Optical Aerial Images,” Remote Sensing, vol. 13, no. 8, p. 1440, 2021.

[15]	B. Adriano et al., “Learning from multimodal and multitemporal earth observation data for building damage mapping,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 175, pp. 132-143, 2021/05/01/ 2021.

[16]	Q. Ding, Z. Shao, X. Huang, and O. Altan, “DSA-Net: A novel deeply supervised attention-guided network for building change detection in high-resolution remote sensing images,” International Journal of Applied Earth Observation and Geoinformation, vol. 105, p. 102591, 2021/12/25/ 2021.

[17]	S. Fang, K. Li, J. Shao, and Z. Li, “SNUNet-CD: A Densely Connected Siamese Network for Change Detection of VHR Images,” IEEE Geoscience and Remote Sensing Letters, pp. 1-5, 2021.

[18]	Q. Guo, J. Zhang, S. Zhu, C. Zhong, and Y. Zhang, “Deep Multiscale Siamese Network with Parallel Convolutional Structure and Self-Attention for Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, pp. 1-1, 2021.

[19]	J. Huang, Q. Shen, M. Wang, and M. Yang, “Multiple Attention Siamese Network for High-Resolution Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, pp. 1-1, 2021.

[20]	X. Jiang, S. Xiang, M. Wang, and P. Tang, “Dual-Pathway Change Detection Network Based on the Adaptive Fusion Module,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2021.

[21]	X. Li, Z. Du, Y. Huang, and Z. Tan, “A deep translation (GAN) based change detection network for optical and SAR remote sensing images,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 179, pp. 14-34, 2021/09/01/ 2021.

[22]	X. Li, M. He, H. Li, and H. Shen, “A Combined Loss-Based Multiscale Fully Convolutional Network for High-Resolution Remote Sensing Image Change Detection,” IEEE Geoscience and Remote Sensing Letters, pp. 1-5, 2021.

[23]	F. Pan, Z. Wu, Q. Liu, Y. Xu, and Z. Wei, “DCFF-Net: A Densely Connected Feature Fusion Network for Change Detection in High-Resolution Remote Sensing Images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 14, pp. 11974-11985, 2021.

[24]	M. Papadomanolaki, M. Vakalopoulou, and K. Karantzalos, “A Deep Multitask Learning Framework Coupling Semantic Segmentation and Fully Convolutional LSTM Networks for Urban Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 59, no. 9, pp. 7651-7668, 2021.

[25]	D. Peng, L. Bruzzone, Y. Zhang, H. Guan, and P. He, “SCDNET: A novel convolutional network for semantic change detection in high resolution optical remote sensing imagery,” International Journal of Applied Earth Observation and Geoinformation, vol. 103, p. 102465, 2021/12/01/ 2021.

[26]	D. Wang, X. Chen, M. Jiang, S. Du, B. Xu, and J. Wang, “ADS-Net:An Attention-Based deeply supervised network for remote sensing image change detection,” International Journal of Applied Earth Observation and Geoinformation, vol. 101, p. 102348, 2021/09/01/ 2021.

[27]	H. Wei, R. Chen, C. Yu, H. Yang, and S. An, “BASNet: A Boundary-Aware Siamese Network for Accurate Remote Sensing Change Detection,” IEEE Geoscience and Remote Sensing Letters, pp. 1-1, 2021.

[28]	L. Zhang, X. Hu, M. Zhang, Z. Shu, and H. Zhou, “Object-level change detection with a dual correlation attention-guided detector,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 177, pp. 147-160, 2021/07/01/ 2021.

[29]	X. Zhang et al., “DifUnet++: A Satellite Images Change Detection Network Based on Unet++ and Differential Pyramid,” IEEE Geoscience and Remote Sensing Letters, pp. 1-5, 2021.

[30]	Z. Zheng, Y. Wan, Y. Zhang, S. Xiang, D. Peng, and B. Zhang, “CLNet: Cross-layer convolutional neural network for change detection in optical remote sensing imagery,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 175, pp. 247-267, 2021/05/01/ 2021.

[31]	Q. Zhu et al., “Land-Use/Land-Cover change detection based on a Siamese global learning framework for high spatial resolution remote sensing imagery,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 184, pp. 63-78, 2022/02/01/ 2022.

[32]	Q. Ke and P. Zhang, “CS-HSNet: A Cross-Siamese Change Detection Network Based on Hierarchical-Split Attention,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 14, pp. 9987-10002, 2021.

[33]	B. Bai, W. Fu, T. Lu, and S. Li, “Edge-Guided Recurrent Convolutional Neural Network for Multitemporal Remote Sensing Image Building Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, pp. 1-13, 2021.

[34]	K. S. Basavaraju, N. Sravya, S. Lal, J. Nalini, C. S. Reddy, and F. Dell’Acqua, “UCDNet: A Deep Learning Model for Urban Change Detection From Bi-Temporal Multispectral Sentinel-2 Satellite Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-10, 2022.

[35]	P. Chen, B. Zhang, D. Hong, Z. Chen, X. Yang, and B. Li, “FCCDN: Feature constraint network for VHR image change detection,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 187, pp. 101-119, 2022/05/01/ 2022.

[36]	T. Chen, Z. Lu, Y. Yang, Y. Zhang, B. Du, and A. Plaza, “A Siamese Network Based U-Net for Change Detection in High Resolution Remote Sensing Images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 2357-2369, 2022.

[37]	G. Cheng, G. Wang, and J. Han, “ISNet: Towards Improving Separability for Remote Sensing Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-11, 2022.

[38]	Y. Deng et al., “Feature-Guided Multitask Change Detection Network,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 9667-9679, 2022.

[39]	M. Han, R. Li, and C. Zhang, “LWCDNet: A Lightweight Fully Convolution Network for Change Detection in Optical Remote Sensing Imagery,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2022.

[40]	H. He, Y. Chen, M. Li, and Q. Chen, “ForkNet: Strong Semantic Feature Representation and Subregion Supervision for Accurate Remote Sensing Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 2142-2153, 2022.

[41]	J. Jiang, J. Xiang, E. Yan, Y. Song, and D. Mo, “Forest-CD: Forest Change Detection Network Based on VHR Images,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2022.

[42]	T. Lei, D. Xue, H. Ning, S. Yang, Z. Lv, and A. K. Nandi, “Local and Global Feature Learning With Kernel Scale-Adaptive Attention Network for VHR Remote Sensing Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 7308-7322, 2022.

[43]	Z. Li, C. Yan, Y. Sun, and Q. Xin, “A Densely Attentive Refinement Network for Change Detection Based on Very-High-Resolution Bitemporal Remote Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-18, 2022.

[44]	A. Raza, H. Huo, and T. Fang, “EUNet-CD: Efficient UNet++ for Change Detection of Very High-Resolution Remote Sensing Images,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2022.

[45]	X. Xiang, D. Tian, N. Lv, and Q. Yan, “FCDNet: A Change Detection Network Based on Full-Scale Skip Connections and Coordinate Attention,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2022.

[46]	C. Zhang, L. Wang, S. Cheng, and Y. Li, “SwinSUNet: Pure Transformer Network for Remote Sensing Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-13, 2022.

[47]	Z. Chen et al., “EGDE-Net: A building change detection method for high-resolution remote sensing imagery based on edge guidance and differential enhancement,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 191, pp. 203-222, 2022/09/01/ 2022.

[48]	X. Zhang et al., “SMD-Net: Siamese Multi-Scale Difference-Enhancement Network for Change Detection in Remote Sensing,” Remote Sensing, vol. 14, no. 7, p. 1580, 2022.

[49]	K. Jiang, W. Zhang, J. Liu, F. Liu, and L. Xiao, “Joint Variation Learning of Fusion and Difference Features for Change Detection in Remote Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-18, 2022.

[50]	T. Lei et al., “Difference Enhancement and Spatial–Spectral Nonlocal Network for Change Detection in VHR Remote Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-13, 2022.

[51]	Q. Li, R. Zhong, X. Du, and Y. Du, “TransUNetCD: A Hybrid Transformer Network for Change Detection in Optical Remote-Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-19, 2022.

[52]	Z. Lv, F. Wang, G. Cui, J. A. Benediktsson, T. Lei, and W. Sun, “Spatial–Spectral Attention Network Guided With Change Magnitude Image for Land Cover Change Detection Using Remote Sensing Images,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-12, 2022.

[53]	G. Pei and L. Zhang, “Feature Hierarchical Differentiation for Remote Sensing Image Change Detection,” IEEE Geoscience and Remote Sensing Letters, vol. 19, pp. 1-5, 2022.

[54]	Q. Shu, J. Pan, Z. Zhang, and M. Wang, “DPCC-Net: Dual-perspective change contextual network for change detection in high-resolution remote sensing images,” International Journal of Applied Earth Observation and Geoinformation, vol. 112, p. 102940, 2022/08/01/ 2022.

[55]	D. Song, Y. Dong, and X. Li, “Context and Difference Enhancement Network for Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 9457-9467, 2022.

[56]	L. Wang and H. Li, “HMCNet: Hybrid Efficient Remote Sensing Images Change Detection Network Based on Cross-Axis Attention MLP and CNN,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-14, 2022.

[57]	J. Yuan, L. Wang, and S. Cheng, “STransUNet: A Siamese TransUNet-Based Remote Sensing Image Change Detection Network,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 15, pp. 9241-9253, 2022.

[58]	C. Zhang et al., “A domain adaptation neural network for change detection with heterogeneous optical and SAR remote sensing images,” International Journal of Applied Earth Observation and Geoinformation, vol. 109, p. 102769, 2022/05/01/ 2022.

[59]	H. Zheng et al., “HFA-Net: High frequency attention siamese network for building change detection in VHR remote sensing images,” Pattern Recognition, vol. 129, p. 108717, 2022/09/01/ 2022.

[60]	Z. Li, C. Tang, L. Wang, and A. Y. Zomaya, “Remote Sensing Change Detection via Temporal Feature Interaction and Guided Refinement,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-11, 2022.

[61]	Q. Shen, J. Huang, M. Wang, S. Tao, R. Yang, and X. Zhang, “Semantic feature-constrained multitask siamese network for building change detection in high-spatial-resolution remote sensing imagery,” ISPRS Journal of Photogrammetry and Remote Sensing, vol. 189, pp. 78-94, 2022/07/01/ 2022.

[62]	H. Xia, Y. Tian, L. Zhang, and S. Li, “A Deep Siamese Postclassification Fusion Network for Semantic Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 60, pp. 1-16, 2022.

[63]	Z. Fu, J. Li, Z. Chen, L. Ren, and Z. Hua, “DAFT: Differential Feature Extraction Network Based on Adaptive Frequency Transformer for Remote Sensing Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 5061-5076, 2023.

[64]	W. Gao, Y. Sun, X. Han, Y. Zhang, L. Zhang, and Y. Hu, “AMIO-Net: An Attention-Based Multiscale Input–Output Network for Building Change Detection in High-Resolution Remote Sensing Images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 2079-2093, 2023.

[65]	S. Holail, T. Saleh, X. Xiao, and D. Li, “AFDE-Net: Building Change Detection Using Attention-Based Feature Differential Enhancement for Satellite Imagery,” IEEE Geoscience and Remote Sensing Letters, vol. 20, pp. 1-5, 2023.

[66]	J. Li, S. Li, and F. Wang, “Adaptive Fusion NestedUNet for Change Detection Using Optical Remote Sensing Images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 5374-5386, 2023.

[67]	W. Li, L. Xue, X. Wang, and G. Li, “ConvTransNet: A CNN–Transformer Network for Change Detection With Multiscale Global–Local Representations,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-15, 2023.

[68]	Z. Li et al., “Lightweight Remote Sensing Change Detection With Progressive Feature Aggregation and Supervised Attention,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-12, 2023.

[69]	Z. Lv, P. Zhong, W. Wang, Z. You, and N. Falco, “Multiscale Attention Network Guided With Change Gradient Image for Land Cover Change Detection Using Remote Sensing Images,” IEEE Geoscience and Remote Sensing Letters, vol. 20, pp. 1-5, 2023.

[70]	X. Tang, T. Zhang, J. Ma, X. Zhang, F. Liu, and L. Jiao, “WNet: W-Shaped Hierarchical Network for Remote-Sensing Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-14, 2023.

[71]	J. Wang et al., “SSCFNet: A Spatial-Spectral Cross Fusion Network for Remote Sensing Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 4000-4012, 2023.

[72]	X. Xu, J. Li, and Z. Chen, “TCIANet: Transformer-Based Context Information Aggregation Network for Remote Sensing Image Change Detection,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 1951-1971, 2023.

[73]	L. Yan and J. Jiang, “A Hybrid Siamese Network With Spatiotemporal Enhancement and Two-Level Feature Fusion for Remote Sensing Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-17, 2023.

[74]	H. Yin et al., “Attention-guided siamese networks for change detection in high resolution remote sensing images,” International Journal of Applied Earth Observation and Geoinformation, vol. 117, p. 103206, 2023/03/01/ 2023.

[75]	Y. Feng, J. Jiang, H. Xu, and J. Zheng, “Change Detection on Remote Sensing Images Using Dual-Branch Multilevel Intertemporal Network,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-15, 2023.

[76]	M. Zhang, Q. Li, Y. Miao, Y. Yuan, and Q. Wang, “Difference-Guided Aggregation Network With Multiimage Pixel Contrast for Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-14, 2023.

[77]	X. Zhang, S. Cheng, L. Wang, and H. Li, “Asymmetric Cross-Attention Hierarchical Network Based on CNN and Transformer for Bitemporal Remote Sensing Images Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-15, 2023.

[78]	C. Zhao et al., “High-Resolution Remote Sensing Bitemporal Image Change Detection Based on Feature Interaction and Multitask Learning,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-14, 2023.

[79]	Y. Zhao, P. Chen, Z. Chen, Y. Bai, Z. Zhao, and X. Yang, “A Triple-Stream Network With Cross-Stage Feature Fusion for High-Resolution Image Change Detection,” IEEE Transactions on Geoscience and Remote Sensing, vol. 61, pp. 1-17, 2023.

[80]	Z. Huang and H. You, “MFSFNet: Multi-Scale Feature Subtraction Fusion Network for Remote Sensing Image Change Detection,” Remote Sensing, vol. 15, no. 15, p. 3740, 2023.

[81]	C. Han, C. Wu, H. Guo, M. Hu, and H. Chen, “HANet: A hierarchical attention network for change detection with bi-temporal very-high-resolution remote sensing images,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, pp. 1-17, 2023.

[82]	H. Zhong and C. Wu, "T-UNet: Triplet UNet for Change Detection in High-Resolution Remote Sensing Images," Available: https://arxiv.org/abs/2308.02356

[83]	C. Han, C. Wu, H. Guo, M. Hu, J. Li, and H. Chen, “Change Guiding Network: Incorporating Change Prior to Guide Change Detection in Remote Sensing Imagery,” IEEE Journal of Selected Topics in Applied Earth Observations and Remote Sensing, vol. 16, pp. 8395-8407, 2023.

[84]	H. Guo, X. Su, C. Wu, B. Du, and L. Zhang, "SAAN: Similarity-aware attention flow network for change detection with VHR remote sensing images," Available: https://arxiv.org/abs/2308.14570

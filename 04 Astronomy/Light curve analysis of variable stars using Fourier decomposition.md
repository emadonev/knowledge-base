---
annotation-target: Light curve analysis of variable stars using Fourier decomposition.pdf
---




>%%
>```annotation-json
>{"created":"2023-08-06T08:03:47.554Z","updated":"2023-08-06T08:03:47.554Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":649,"end":816},{"type":"TextQuoteSelector","exact":"e show the use of principal component analysis (PCA) and Fourier decomposition (FD) method as tools for variable stardiagnostics and compare their relative performance","prefix":"lass in an automated way.Aims. W","suffix":" in studying the changes in the "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==e show the use of principal component analysis (PCA) and Fourier decomposition (FD) method as tools for variable stardiagnostics and compare their relative performance== *
>%%LINK%%[[#^hzg7dg6eghm|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^hzg7dg6eghm


>%%
>```annotation-json
>{"created":"2023-08-06T08:04:55.312Z","text":"So, this would mean that the PCA method is better than the FD method. \n\nFind out how PCA's work, and try to implement in Python! But, if you decide to use FD for the actual period calculation (the lomb-scargle thing) then use PCA for categorizing light curves into types.","updated":"2023-08-06T08:04:55.312Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":1424,"end":2308},{"type":"TextQuoteSelector","exact":"We show that in general, the first few principal components (PCs) are enough to reconstruct the original light curves com-pared to FD method where 2 to 3 times more number of parameters are required to satisfactorily reconstruct the light curves. Thecomputation of required number of Fourier parameters on the average needs 20 times more CPU time than the computation of requirednumber of PCs. Therefore, PCA does have some advantage over the FD method in analysing the variable stars in a larger database.However in some cases, particularly in finding the resonances in Fundamental mode (FU) Cepheids, the PCA results show no distinctadvantages over the FD method. We also demonstrate that the PCA technique can be used to classify variables into different variabilityclasses in an automated, unsupervised way, a feature that has immense potential for larger databases of the future.","prefix":"ed as input to the PCA.Results. ","suffix":"Conclusions.Key words. Methods: "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==We show that in general, the first few principal components (PCs) are enough to reconstruct the original light curves com-pared to FD method where 2 to 3 times more number of parameters are required to satisfactorily reconstruct the light curves. Thecomputation of required number of Fourier parameters on the average needs 20 times more CPU time than the computation of requirednumber of PCs. Therefore, PCA does have some advantage over the FD method in analysing the variable stars in a larger database.However in some cases, particularly in finding the resonances in Fundamental mode (FU) Cepheids, the PCA results show no distinctadvantages over the FD method. We also demonstrate that the PCA technique can be used to classify variables into different variabilityclasses in an automated, unsupervised way, a feature that has immense potential for larger databases of the future.== *
>%%LINK%%[[#^ad0uibzf31h|show annotation]]
>%%COMMENT%%
>So, this would mean that the PCA method is better than the FD method. 
>
>Find out how PCA's work, and try to implement in Python! But, if you decide to use FD for the actual period calculation (the lomb-scargle thing) then use PCA for categorizing light curves into types.
>%%TAGS%%
>
^ad0uibzf31h


>%%
>```annotation-json
>{"created":"2023-08-06T08:09:00.593Z","text":"I think that even with multiprocessing that this wouldn't work. ","updated":"2023-08-06T08:09:00.593Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":4216,"end":4433},{"type":"TextQuoteSelector","exact":" Fourier decomposi-tion by itself is not perfectly suitable for classification of variablestars in large databases as the method works for individual stars,but can be used as a preprocessor for other automated schemes","prefix":"4, Tanvir et al. 2005). However,","suffix":"(Kanbur et al. 2002, Kanbur & Ma"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==Fourier decomposi-tion by itself is not perfectly suitable for classification of variablestars in large databases as the method works for individual stars,but can be used as a preprocessor for other automated schemes== *
>%%LINK%%[[#^04sk1gojdlfj|show annotation]]
>%%COMMENT%%
>I think that even with multiprocessing that this wouldn't work. 
>%%TAGS%%
>
^04sk1gojdlfj


>%%
>```annotation-json
>{"created":"2023-08-06T08:12:06.422Z","text":"**What does this mean exactly?**\n\nDoes this mean that in order to fit a light curve you need the period of the light curve or? It turns out that **the period is necessary for this, so this paper can be used in a later stage!**","updated":"2023-08-06T08:12:06.422Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":4496,"end":4675},{"type":"TextQuoteSelector","exact":"The principal component analysis transforms the originaldata set of variables by way of an orthogonal transformation to anew set of uncorrelated variables or principal components.","prefix":"ariani 2004, Sarro et al. 2009).","suffix":" Thetechnique amounts to a strai"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==The principal component analysis transforms the originaldata set of variables by way of an orthogonal transformation to anew set of uncorrelated variables or principal components.== *
>%%LINK%%[[#^80hzmqt19qd|show annotation]]
>%%COMMENT%%
>**What does this mean exactly?**
>
>Does this mean that in order to fit a light curve you need the period of the light curve or? It turns out that **the period is necessary for this, so this paper can be used in a later stage!**
>%%TAGS%%
>
^80hzmqt19qd


>%%
>```annotation-json
>{"created":"2023-08-06T08:13:29.233Z","updated":"2023-08-06T08:13:29.233Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":5290,"end":5544},{"type":"TextQuoteSelector","exact":"Therehave been a number of studies on the use of PCA in analyzingCepheid light curves (Kanbur et al. 2002) and RR Lyrae lightcurves (Kanbur & Mariani 2004). In both these studies, the inputdata to the PCA are the Fourier coefficients rather than the ligh","prefix":", Folkes, Lahav & Maddox 1996). ","suffix":"t2 Deb and Singh: Light curve an"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==Therehave been a number of studies on the use of PCA in analyzingCepheid light curves (Kanbur et al. 2002) and RR Lyrae lightcurves (Kanbur & Mariani 2004). In both these studies, the inputdata to the PCA are the Fourier coefficients rather than the ligh== *
>%%LINK%%[[#^22ksw1t6j69|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^22ksw1t6j69


>%%
>```annotation-json
>{"created":"2023-08-06T08:13:38.842Z","updated":"2023-08-06T08:13:38.842Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":6210,"end":6384},{"type":"TextQuoteSelector","exact":"curves themselves. Nevertheless, it was noted that the PCA wasable to reproduce the light curves with about half the number ofparameters (PCs) needed by the Fourier technique","prefix":"yrzykowski et al. (2004) 1404 VB","suffix":". We may re-call that in the PCA"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==curves themselves. Nevertheless, it was noted that the PCA wasable to reproduce the light curves with about half the number ofparameters (PCs) needed by the Fourier technique== *
>%%LINK%%[[#^49h3286eoqc|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^49h3286eoqc


>%%
>```annotation-json
>{"created":"2023-08-06T08:15:33.719Z","updated":"2023-08-06T08:15:33.719Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":7925,"end":8115},{"type":"TextQuoteSelector","exact":"Therefore it is not meaning-ful to use Fourier coefficients as input to the PCA when lightcurves of a large number of variable stars having different vari-ability classes are to be analysed.","prefix":"he true light curve structures. ","suffix":" We demonstrate this fact withth"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==Therefore it is not meaning-ful to use Fourier coefficients as input to the PCA when lightcurves of a large number of variable stars having different vari-ability classes are to be analysed.== *
>%%LINK%%[[#^pcy60fy2gpg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^pcy60fy2gpg


>%%
>```annotation-json
>{"created":"2023-08-06T08:17:05.096Z","updated":"2023-08-06T08:17:05.096Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":9071,"end":9207},{"type":"TextQuoteSelector","exact":"PCA, all the light curve data can be processedand analysed in one go if all the phased light curve data canbe made of similar dimensions","prefix":"CA over the FDmethod is that in ","suffix":" as we shall demonstrate later,w"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==PCA, all the light curve data can be processedand analysed in one go if all the phased light curve data canbe made of similar dimensions== *
>%%LINK%%[[#^45zlwpkb68c|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^45zlwpkb68c


>%%
>```annotation-json
>{"created":"2023-08-06T08:29:16.407Z","text":"This is super important and very necessary for me!","updated":"2023-08-06T08:29:16.407Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":12685,"end":12857},{"type":"TextQuoteSelector","exact":"PCA can be used forpreliminary classification of the variable stars such as classifica-tion between pulsating stars and Eclipsing binaries and differentvariability classes.","prefix":"f its use for future databases. ","suffix":"We present the Fourier decomposi"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==PCA can be used forpreliminary classification of the variable stars such as classifica-tion between pulsating stars and Eclipsing binaries and differentvariability classes.== *
>%%LINK%%[[#^q0ba2jq1aj|show annotation]]
>%%COMMENT%%
>This is super important and very necessary for me!
>%%TAGS%%
>
^q0ba2jq1aj


>%%
>```annotation-json
>{"created":"2023-08-06T08:29:39.658Z","text":"This algorithm is kind of like a *neural network*, because it uses both **gradient descent and the gauss-newton method**, which is a method where it calculates the non-linear least squares and assumes that the residuals follow a Gaussian distribution.\n\nCombined with the fourier decomposition, this algorithm enables us to find the correct fourier series which describes our light curve!","updated":"2023-08-06T08:29:39.658Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":12872,"end":12975},{"type":"TextQuoteSelector","exact":"Fourier decomposition technique usingLevenberg-Marquardt algorithm for non-linear least square fit-ting","prefix":"iability classes.We present the ","suffix":" (Press et al. 1992) in Sect. 2."}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==Fourier decomposition technique usingLevenberg-Marquardt algorithm for non-linear least square fit-ting== *
>%%LINK%%[[#^mhny59t1f6f|show annotation]]
>%%COMMENT%%
>This algorithm is kind of like a *neural network*, because it uses both **gradient descent and the gauss-newton method**, which is a method where it calculates the non-linear least squares and assumes that the residuals follow a Gaussian distribution.
>
>Combined with the fourier decomposition, this algorithm enables us to find the correct fourier series which describes our light curve!
>%%TAGS%%
>
^mhny59t1f6f


>%%
>```annotation-json
>{"created":"2023-08-06T08:31:59.603Z","text":"So, this formula basically sums all of the sine waves and the cos waves in order to get the final \"wave\" which is made up of these components. This equation is also called the **fourier series!**","updated":"2023-08-06T08:31:59.603Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":13713,"end":13770},{"type":"TextQuoteSelector","exact":"m(t) = A0 +N∑i=1ai cos(iω(t −t0)) +N∑i=1bi sin(iω(t −t0))","prefix":" a sum of cosine and sineseries:","suffix":", (1)where m(t) is the observed "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==m(t) = A0 +N∑i=1ai cos(iω(t −t0)) +N∑i=1bi sin(iω(t −t0))== *
>%%LINK%%[[#^3y2jm83pv9q|show annotation]]
>%%COMMENT%%
>So, this formula basically sums all of the sine waves and the cos waves in order to get the final "wave" which is made up of these components. This equation is also called the **fourier series!**
>%%TAGS%%
>
^3y2jm83pv9q


>%%
>```annotation-json
>{"created":"2023-08-06T08:41:23.502Z","text":"So, this equation is the same as the original Fourier decomposition, with a little twist.\n\nSo, it tries to tell us how our light curve behaves based on the average magnitude, the summation of all the harmonics of our light curve, which are described by the amplitude of every harmonic and the shift in harmonics. The relative fourier parameters are the *relative amplitude and phase*. This is very important since we are **phasing** light curves. The relative phase It provides a measure of how shifted or delayed the ith harmonic is in relation to the primary frequency component. The relative amplitude gives the normalized measure of how strong the ith harmonic is compared to the base one. \n\nThe reason why **there is no sine in the new equation**, is because of trigonometric identities, where we we managed to pack everything into a cosine term with **a phase shift.** ","updated":"2023-08-06T08:41:23.502Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":14701,"end":14735},{"type":"TextQuoteSelector","exact":"m(t) = A0 +N∑i=1Aicos[2πiΦ(t) +φi]","prefix":"Φ(t)) +N∑i=1bi sin(2πiΦ(t)), (4)","suffix":", (5)with relative Fourier param"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==m(t) = A0 +N∑i=1Aicos[2πiΦ(t) +φi]== *
>%%LINK%%[[#^v223lr8yhc|show annotation]]
>%%COMMENT%%
>So, this equation is the same as the original Fourier decomposition, with a little twist.
>
>So, it tries to tell us how our light curve behaves based on the average magnitude, the summation of all the harmonics of our light curve, which are described by the amplitude of every harmonic and the shift in harmonics. The relative fourier parameters are the *relative amplitude and phase*. This is very important since we are **phasing** light curves. The relative phase It provides a measure of how shifted or delayed the ith harmonic is in relation to the primary frequency component. The relative amplitude gives the normalized measure of how strong the ith harmonic is compared to the base one. 
>
>The reason why **there is no sine in the new equation**, is because of trigonometric identities, where we we managed to pack everything into a cosine term with **a phase shift.** 
>%%TAGS%%
>
^v223lr8yhc


>%%
>```annotation-json
>{"created":"2023-08-06T08:42:21.071Z","text":"This is used to determine how high of a degree our fourier decomposition should be. \n\nExplanation: \nSo, p is trying to tell us how do the residuals of our light curve behave. Is there some pattern or is it random? In the numerator, it sums up all of the products between the jth residual and the next residual. The denominator looks a lot like variance! It tells us how far away each residual is from the mean residual squared, or how spread out our errors are. This looks more and more like a loss function! \n\n**LIGHT CURVE ANALYSIS**\nFrom ChatGPT:\nIn the context of light curve analysis, if ρ is close to 1 or -1, it indicates that the residuals have a strong pattern, suggesting that the Fourier decomposition might be missing some periodic component. If ρ is close to 0, it indicates that the residuals are more random, suggesting that the Fourier decomposition has captured the main periodic components of the light curve.","updated":"2023-08-06T08:42:21.071Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":16228,"end":16272},{"type":"TextQuoteSelector","exact":"ρ:=∑nj=1(vj − ̄v)(vj+1 − ̄v)∑nj=1 (vj − ̄v)2","prefix":"t of noiseonly. It as defined as","suffix":"where v j is the jth residual,  "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==ρ:=∑nj=1(vj − ̄v)(vj+1 − ̄v)∑nj=1 (vj − ̄v)2== *
>%%LINK%%[[#^pl6lebjcyd|show annotation]]
>%%COMMENT%%
>This is used to determine how high of a degree our fourier decomposition should be. 
>
>Explanation: 
>So, p is trying to tell us how do the residuals of our light curve behave. Is there some pattern or is it random? In the numerator, it sums up all of the products between the jth residual and the next residual. The denominator looks a lot like variance! It tells us how far away each residual is from the mean residual squared, or how spread out our errors are. This looks more and more like a loss function! 
>
>**LIGHT CURVE ANALYSIS**
>From ChatGPT:
>In the context of light curve analysis, if ρ is close to 1 or -1, it indicates that the residuals have a strong pattern, suggesting that the Fourier decomposition might be missing some periodic component. If ρ is close to 0, it indicates that the residuals are more random, suggesting that the Fourier decomposition has captured the main periodic components of the light curve.
>%%TAGS%%
>
^pl6lebjcyd


>%%
>```annotation-json
>{"created":"2023-08-06T08:52:06.422Z","text":"This equation is key to understanding the equation above. This equation describes the difference between the original light curve and the Fourier approximation, kind of like the loss function in a neural network. It substracts the approximation from the actual behavior. ","updated":"2023-08-06T08:52:06.422Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":16468,"end":16506},{"type":"TextQuoteSelector","exact":"v =m(t) −[A0 +N∑i=1Aicos(2πiΦ(t) +φi)]","prefix":"iduals of the fitted light curve","suffix":"It should be noted that for the "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==v =m(t) −[A0 +N∑i=1Aicos(2πiΦ(t) +φi)]== *
>%%LINK%%[[#^l5cvuqw46b|show annotation]]
>%%COMMENT%%
>This equation is key to understanding the equation above. This equation describes the difference between the original light curve and the Fourier approximation, kind of like the loss function in a neural network. It substracts the approximation from the actual behavior. 
>%%TAGS%%
>
^l5cvuqw46b


>%%
>```annotation-json
>{"created":"2023-08-06T08:59:08.365Z","text":"I can use this as reference for my light curves, although I do not know their types. ","updated":"2023-08-06T08:59:08.365Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":17626,"end":17794},{"type":"TextQuoteSelector","exact":"The optimal order of thefit for RRc, RRab, FU Cepheids (OGLE), First Overtone (FO)Cepheids, Eclipsing binaries and Mira variables are 3, 5, 12, 10,4 and 4 respectively.","prefix":"Baart’s condition is satisfied. ","suffix":" The longer period data for FU C"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==The optimal order of thefit for RRc, RRab, FU Cepheids (OGLE), First Overtone (FO)Cepheids, Eclipsing binaries and Mira variables are 3, 5, 12, 10,4 and 4 respectively.== *
>%%LINK%%[[#^8p0abr7z87o|show annotation]]
>%%COMMENT%%
>I can use this as reference for my light curves, although I do not know their types. 
>%%TAGS%%
>
^8p0abr7z87o


>%%
>```annotation-json
>{"created":"2023-08-06T09:03:15.605Z","text":"Using this method we minimize dimensionality while still regaining all of the major trends. It rotates our data and represents our data in some new variables. The first variable represents the strongest trend, the second variable the second-strongest trend, etc. ","updated":"2023-08-06T09:03:15.605Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":19056,"end":19371},{"type":"TextQuoteSelector","exact":"The principal component analysis transforms the original set ofp variables by an orthogonal transformation to a new set of un-correlated variables or principal components (PCs). It involvesa simple rotation from the original axes to the new ones result-ing in principal components in decreasing order of importance.","prefix":"n3. PRINCIPAL COMPONENT ANALYSIS","suffix":"The first few q components (q ≪ "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==The principal component analysis transforms the original set ofp variables by an orthogonal transformation to a new set of un-correlated variables or principal components (PCs). It involvesa simple rotation from the original axes to the new ones result-ing in principal components in decreasing order of importance.== *
>%%LINK%%[[#^opzvg3allzh|show annotation]]
>%%COMMENT%%
>Using this method we minimize dimensionality while still regaining all of the major trends. It rotates our data and represents our data in some new variables. The first variable represents the strongest trend, the second variable the second-strongest trend, etc. 
>%%TAGS%%
>
^opzvg3allzh


>%%
>```annotation-json
>{"created":"2023-08-06T09:12:23.931Z","text":"THE TRANSFORMATION\n------------\nSo, m_i_j is the magnitude of the jth point in the ith light curve.\nn is the number of light curves.\np is the number of observations per light curve.\n\nWe start of by standardizing our light curves.\n1. We create a matrix X, which will store all of our observations for easy access and transformation, since we can utilize vector operations. *Every row is a light curve, and every column an observation or data point.*\n2. We standardize each value so the mean is 0 and the standard deviation is 1, making the PCA easier to handle.\n\nNext up we calculate the mean, or the average magnitude of the j-th observation across all light curves, and the variance of the data or the variance of the j-th observation across all light curves.\n\nThen we calculate the **correlation matrix (C):** this tells us how individual observations are related, and we store the results in a new matrix. If they increase, they have a positive correlation, and the opposite is true. \n\nFinally, we use all of this to create our most significant trend in the data! This is called the **first principal component!**  ","updated":"2023-08-06T09:12:23.931Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":20727,"end":20782},{"type":"TextQuoteSelector","exact":"In the following, we brieflydescribe the transformation","prefix":"002, 2004, Tanvir et al. 2005). ","suffix":".Let mi j be the p magnitudes co"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==In the following, we brieflydescribe the transformation== *
>%%LINK%%[[#^f9z7eruu5oc|show annotation]]
>%%COMMENT%%
>THE TRANSFORMATION
>------------
>So, m_i_j is the magnitude of the jth point in the ith light curve.
>n is the number of light curves.
>p is the number of observations per light curve.
>
>We start of by standardizing our light curves.
>1. We create a matrix X, which will store all of our observations for easy access and transformation, since we can utilize vector operations. *Every row is a light curve, and every column an observation or data point.*
>2. We standardize each value so the mean is 0 and the standard deviation is 1, making the PCA easier to handle.
>
>Next up we calculate the mean, or the average magnitude of the j-th observation across all light curves, and the variance of the data or the variance of the j-th observation across all light curves.
>
>Then we calculate the **correlation matrix (C):** this tells us how individual observations are related, and we store the results in a new matrix. If they increase, they have a positive correlation, and the opposite is true. 
>
>Finally, we use all of this to create our most significant trend in the data! This is called the **first principal component!**  
>%%TAGS%%
>
^f9z7eruu5oc


>%%
>```annotation-json
>{"created":"2023-08-06T09:25:22.390Z","text":"So, how do we go from the first component to a fitted light curve?\n\nFrom ChatGPT:\n**Step 1:** Determine how many principal components (q) you need to capture the essential patterns in your light curves.\n\n**Step 2:** Use the eigenvectors (stored in matrix Eq) of these q components to transform your original data into a new space. This transformation gives you the projection vector Z.\n\n**Step 3:** To get back to the original space (i.e., to reconstruct the light curve), you multiply Z by the transpose of Eq. This gives you a version of the light curve that's been \"fitted\" using the principal components.\n\n**Step 4: **Adjust this fitted light curve to have the original scale and offset by multiplying with s_j √n and adding the mean.\n\nSo, basically using the eigenvectors or the main trends we reconstruct the original light curve and we try to use the fewest number of eigenvectors. ","updated":"2023-08-06T09:25:22.390Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":22038,"end":22241},{"type":"TextQuoteSelector","exact":"We obtain the final light curve xrec by multiplying x withs j√n and adding the mean. Z is a (n ×q) matrix and Eq T is a( q × p) matrix and hence the reconstructed light curve is theoriginal (n ×p) matrix","prefix":" be represented byx =ZEq T. (10)","suffix":".With the phase (Φ) as epoch for"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==We obtain the final light curve xrec by multiplying x withs j√n and adding the mean. Z is a (n ×q) matrix and Eq T is a( q × p) matrix and hence the reconstructed light curve is theoriginal (n ×p) matrix== *
>%%LINK%%[[#^3da3na0nz9g|show annotation]]
>%%COMMENT%%
>So, how do we go from the first component to a fitted light curve?
>
>From ChatGPT:
>**Step 1:** Determine how many principal components (q) you need to capture the essential patterns in your light curves.
>
>**Step 2:** Use the eigenvectors (stored in matrix Eq) of these q components to transform your original data into a new space. This transformation gives you the projection vector Z.
>
>**Step 3:** To get back to the original space (i.e., to reconstruct the light curve), you multiply Z by the transpose of Eq. This gives you a version of the light curve that's been "fitted" using the principal components.
>
>**Step 4: **Adjust this fitted light curve to have the original scale and offset by multiplying with s_j √n and adding the mean.
>
>So, basically using the eigenvectors or the main trends we reconstruct the original light curve and we try to use the fewest number of eigenvectors. 
>%%TAGS%%
>
^3da3na0nz9g


>%%
>```annotation-json
>{"created":"2023-08-06T09:48:47.245Z","text":"So, how do you go about classifying stars by PCA method? Since it is obviously faster than the FD method, I would definitely prefer using it!\n\n1. Apply the PCA method on the light curves. Duh. \n\n2. The next step is to project every light curve to its principal components. This basically means that we see how well the light curve corresponds to the main trends we got from them. For example, score for PC1 (often called the first principal component score) tells you how much a given light curve aligns with the pattern represented by PC1.\n\n3.  Plot this score of PC1 against the log of the periods of the stars. logs help out because it tones down if there are any extreme values and is able to see groups of stars.\n\n4. Using prior knowledge you categorize the stars.","updated":"2023-08-06T09:48:47.245Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":31292,"end":31313},{"type":"TextQuoteSelector","exact":"4.1.3. Classification","prefix":"D and PCA techniques is similar.","suffix":"We now explore the possibility o"}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==4.1.3. Classification== *
>%%LINK%%[[#^aqmkx4h41ro|show annotation]]
>%%COMMENT%%
>So, how do you go about classifying stars by PCA method? Since it is obviously faster than the FD method, I would definitely prefer using it!
>
>1. Apply the PCA method on the light curves. Duh. 
>
>2. The next step is to project every light curve to its principal components. This basically means that we see how well the light curve corresponds to the main trends we got from them. For example, score for PC1 (often called the first principal component score) tells you how much a given light curve aligns with the pattern represented by PC1.
>
>3.  Plot this score of PC1 against the log of the periods of the stars. logs help out because it tones down if there are any extreme values and is able to see groups of stars.
>
>4. Using prior knowledge you categorize the stars.
>%%TAGS%%
>
^aqmkx4h41ro


>%%
>```annotation-json
>{"created":"2023-08-06T09:57:12.440Z","text":"I would definitely use PCA for classifying all of the stars, but for individual analysis for when things get sticky I could use FD for a maybe more precise result.","updated":"2023-08-06T09:57:12.440Z","document":{"title":"","link":[{"href":"urn:x-pdf:e08675f70a39d8739c1c095e3d7ec404"},{"href":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf"}],"documentFingerprint":"e08675f70a39d8739c1c095e3d7ec404"},"uri":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","target":[{"source":"vault:/Light curve analysis of variable stars using Fourier decomposition.pdf","selector":[{"type":"TextPositionSelector","start":38357,"end":38502},{"type":"TextQuoteSelector","exact":"We have also demonstrated the ability of PCA and its distinctadvantage over the FD method in classifying stars into differentvariability classes.","prefix":"ort period objects ofthis class.","suffix":" Although alternative automated "}]}]}
>```
>%%
>*%%HIGHLIGHT%% ==We have also demonstrated the ability of PCA and its distinctadvantage over the FD method in classifying stars into differentvariability classes.== *
>%%LINK%%[[#^cnaefl0sgss|show annotation]]
>%%COMMENT%%
>I would definitely use PCA for classifying all of the stars, but for individual analysis for when things get sticky I could use FD for a maybe more precise result.
>%%TAGS%%
>
^cnaefl0sgss

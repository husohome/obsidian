# Dissertation Dumps
#dissertation #dump

1. short-form development
	1. is important, and was sometimes discouraged [[on the sins of short-form development#^1d478b]]
	2. short forms are developed as a tool for
		1. more efficient testing (time saving) [[short comings of shortened tests#^f4b6db]]
		2. screening
		3. adaptation for children
			1. e.g., [[short comings of shortened tests#^3dfb81]]]
0. what has not been done before:
	1. machine learning as part of the short-form development is probably a recent practice
		1. well there actually is
			1. [[short-form development using machine learning]]
			2. [[shortening big five using elastic net]] (2021)
		2. there is, however, adaptive (tailored) testing using machine learning
	2. no short-form development has considered machine learning as an approach
1. maybe it's good to point out the[[short comings of shortened tests]]
	1. expert judgment and statistical overview are faulty

1. we are applying the neural network to a case where you've shortened a test 
	1. usually short form development involves only item selection (factor-analytic approach)
		1. maybe a systematic review of short form development should be cited here? can't find
		3. found this [[on the sins of short-form development]]
		4. this is really useful review [[short comings of shortened tests]]
	2. you usually choose the most representative items by factor loading but the r-squared is always lower and the correlation between the short-form and the full format usually isn't that astoundingly good
		1. what is a good short form? usually correlation? - yes
			1. [[short comings of shortened tests#^4d49c9]]
		2. what is factually the standard for good short form in education?
			1. state how neural networks beat the "state-of-the-art" performance of a short-form
	3. CMPA is especially difficult, because not only is it a short form scenario, but the formats are different and there are so many categories
	4. thus, if we can solve the problem at hand, our research is really generalizable to many situations
	5. say we propose a few steps and say we'll explain some of them later:
		1. no matter how you choose the items, once you've chosen the items, predict the results with neural networks.
		2. to make evaluating the neural network easier, make it categorical
		3. we recommend using hyperparameter tuning
		4. we recommend using F1-gain/Accuracy-gain to deal with class imbalances
2. review neural networks with the focus on helping the reviewers locate what type of neural networks we are talking about
	1. pinpoint that it is supervised learning, and the most used is RNN in educational data mining and say that ours happens to be a single layer neural network, and say that explain what multilabel means
	3. talk about why neural networks are popular and promising in general and in educational data mining
	4. point out that nobody has used neural networks for test shortening before it's centralized in the subfield of educational data mining (EDM)
	5. summarize key issues
		1. over-fitting 
		2. class imbalances
			1. say we encountered this
		3. hard to find an evaluation criteria
			1. so we designed F1-gain and Precision-gain
		4. hard to find a best model
			1. so we used hyperparameter tuning
3. review CMPA, 
	1. CMPA overview
	2. we are using Likert-type (considering it shortened), but we are not sure how to ...
	3. CMPA provides extra challenges
4. current study
	1. compare MNN with traditional techniques

## Method
1. say we are actually providing a framework
	1. steps are:
		1. no matter how you choose the items, once you've chosen the items, predict the results with neural networks.
		2. to make evaluating the neural network easier, make it categorical
		3. we recommend using hyperparameter tuning
		4. we recommend using F1-gain/Accuracy-gain to deal with class imbalances
2. state the actual steps of hyperparameter tuning

# Python实现朴素贝叶斯垃圾邮件分类

## 项目简介

本项目提供了一个基于Python实现的朴素贝叶斯垃圾邮件分类器。该分类器能够有效地对邮件进行分类，判断其是否为垃圾邮件。通过使用朴素贝叶斯算法，项目实现了对邮件文本的预处理、特征提取、概率计算以及最终的分类决策。

## 功能特点

- **文本预处理**：对邮件文本进行小写转换、符号过滤和数字过滤，确保文本数据的纯净性。
- **特征提取**：将邮件文本分割成单词，并使用集合去重，提取出邮件中的特征词。
- **概率计算**：基于训练数据计算每个特征词在垃圾邮件和正常邮件中出现的概率。
- **分类决策**：利用贝叶斯定理计算邮件属于垃圾邮件和正常邮件的概率，并根据概率大小进行分类。

## 使用方法

1. **数据准备**：准备垃圾邮件和正常邮件的训练数据集。
2. **运行脚本**：运行提供的Python脚本，进行模型训练和测试。
3. **结果分析**：查看分类结果，评估模型的准确性和性能。

## 代码结构

- `replace_num(txt_str)`: 过滤邮件文本中的数字。
- `get_filtered_str(category)`: 获取并预处理指定类别的邮件文本。
- `get_dict_spam_dict_w(spam_email_list)`: 计算垃圾邮件特征词的出现次数。
- `get_dict_ham_dict_w(spam_email_list, ham_email_list)`: 计算正常邮件中垃圾邮件特征词的出现次数。
- `get_X_c1(spam_w_dict, file_name)`: 计算测试邮件属于垃圾邮件的概率。
- `get_X_c2(ham_w_dict, file_name)`: 计算测试邮件属于正常邮件的概率。
- `email_test(spam_w_dict, ham_w_dict)`: 对测试邮件进行分类测试。

## 依赖库

- `os`
- `re`
- `string`
- `math`
- `numpy`

## 注意事项

- 确保训练数据集的质量和数量，以提高分类器的准确性。
- 根据实际需求调整文本预处理和特征提取的策略。

## 参考资料

本项目参考了CSDN博客文章《python实现朴素贝叶斯垃圾邮件分类》，详细介绍了朴素贝叶斯算法的原理和实现步骤。

---

通过本项目，您可以深入了解朴素贝叶斯算法在垃圾邮件分类中的应用，并根据实际需求进行进一步的优化和扩展。

## 下载链接

[Python实现朴素贝叶斯垃圾邮件分类](https://pan.quark.cn/s/027dc6df7107)
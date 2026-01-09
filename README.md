# 运行所有channelMapping测试（包括新增的结果校对测试）
pytest tests/test_channelMapping.py -v

# 仅运行结果校对测试
pytest tests/test_channelMapping.py::TestChannelMapping::test_channelMapping_result_verification -v

# 运行特定数据集的结果校对测试
pytest tests/test_channelMapping.py::TestChannelMapping::test_channelMapping_result_verification[test_data_a-test_data_a] -v

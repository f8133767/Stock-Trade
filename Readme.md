# ʹ��Policy Gradient������������


Trade_env:
	����TradeEnv:
	ͨ��QuandlEnvSrc���¶�ȡgetStock�еĻ�ȡ�����ݣ��õ��͹۹�Ʊ��״̬
	Investorͨ���Լ�����������״̬�����Լ���ʱ����ֽ�cash�Ͳ�λstock��������ÿ�β����ľ��ʲ�����Ϊ�ر�reward

Run��
	��ģ�ͣ���ö�Ӧ����action��observation��
	ͨ��observationѡ��action��observation���뵽�����У����softmax�õ���Ӧ�����ĸ��ʣ�Ȼ��õ��䶯���Ķ���ʽ�ֲ������ո���ѡȡaction
	Action������environment�У�����observation����˴������Ӧ����������actionʩ�Ӻ󣬻���¹���Investor���ֽ�cash�Ͳ�λ״̬���Ӷ��õ��µ�observation_
	��b������ͬʱ���õ���ÿ��observation�£���Ӧaction���õ�reward��һһ��Ӧ
	����ģ�Ͳ�����
	����һϵ��ȡ�õ�reward,���ݸû������ƶ�һ����������Vt
	����ĳobservationѡ��ö����ĸ��ʵ�log �����Ӧ��reward ��˵õ�ÿһ����lossֵ����log��(s_t,a_t )*reward_t
	Lossֵ��ͣ��õ���loss, ���򴫲��󵼣�����ģ��

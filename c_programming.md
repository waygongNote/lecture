*do {...} while(0);*
	two reasons:
	(1) insert several "if (...) break;" in it to replace dangerous "goto" func.
	(2) avoid error or mistake as using #define, 細節不好說, 見下
	ex. #define uip_send(data, len) do { uip_sappdata = (data); uip_slen = (len);} while(0)
	cf. http://blog.csdn.net/coffeecato/article/details/40183887

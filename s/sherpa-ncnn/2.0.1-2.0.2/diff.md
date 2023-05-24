# Comparing `tmp/sherpa_ncnn-2.0.1-cp39-cp39-win_amd64.whl.zip` & `tmp/sherpa_ncnn-2.0.2-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,14 @@
-Zip file size: 3481214 bytes, number of entries: 20
--rw-rw-rw-  2.0 fat   193536 b- defN 23-May-20 09:49 _sherpa_ncnn.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat    90624 b- defN 23-May-20 09:46 kaldi-native-fbank-core.dll
--rw-rw-rw-  2.0 fat    84014 b- defN 23-May-20 09:46 kaldi-native-fbank-core.lib
--rw-rw-rw-  2.0 fat  4323840 b- defN 23-May-20 09:49 ncnn.dll
--rw-rw-rw-  2.0 fat   891598 b- defN 23-May-20 09:49 ncnn.lib
--rw-rw-rw-  2.0 fat   307712 b- defN 23-May-20 09:49 sherpa-ncnn-core.dll
--rw-rw-rw-  2.0 fat   431888 b- defN 23-May-20 09:49 sherpa-ncnn-core.lib
--rw-rw-rw-  2.0 fat       93 b- defN 23-May-20 09:45 sherpa_ncnn/__init__.py
--rw-rw-rw-  2.0 fat     8612 b- defN 23-May-20 09:29 sherpa_ncnn/recognizer.py
--rw-rw-rw-  2.0 fat  4323840 b- defN 23-May-20 09:49 sherpa_ncnn/bin/ncnn.dll
--rw-rw-rw-  2.0 fat    90624 b- defN 23-May-20 09:46 sherpa_ncnn/lib/kaldi-native-fbank-core.dll
--rw-rw-rw-  2.0 fat    84014 b- defN 23-May-20 09:46 sherpa_ncnn/lib/kaldi-native-fbank-core.lib
--rw-rw-rw-  2.0 fat   891598 b- defN 23-May-20 09:49 sherpa_ncnn/lib/ncnn.lib
--rw-rw-rw-  2.0 fat    21504 b- defN 23-May-20 09:49 sherpa_ncnn/lib/sherpa-ncnn-c-api.dll
--rw-rw-rw-  2.0 fat    13524 b- defN 23-May-20 09:49 sherpa_ncnn/lib/sherpa-ncnn-c-api.lib
--rw-rw-rw-  2.0 fat    11560 b- defN 23-May-20 09:49 sherpa_ncnn-2.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2194 b- defN 23-May-20 09:49 sherpa_ncnn-2.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-20 09:49 sherpa_ncnn-2.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       25 b- defN 23-May-20 09:49 sherpa_ncnn-2.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1680 b- defN 23-May-20 09:49 sherpa_ncnn-2.0.1.dist-info/RECORD
-20 files, 11772580 bytes uncompressed, 3478520 bytes compressed:  70.5%
+Zip file size: 3357024 bytes, number of entries: 12
+-rwxr-xr-x  2.0 unx   238624 b- defN 23-May-24 09:55 _sherpa_ncnn.cpython-39-darwin.so
+-rw-r--r--  2.0 unx     8379 b- defN 23-May-24 09:27 sherpa_ncnn/recognizer.py
+-rw-r--r--  2.0 unx       90 b- defN 23-May-24 09:49 sherpa_ncnn/__init__.py
+-rwxr-xr-x  2.0 unx    55744 b- defN 23-May-24 09:55 sherpa_ncnn/lib/libsherpa-ncnn-c-api.dylib
+-rwxr-xr-x  2.0 unx   317824 b- defN 23-May-24 09:55 sherpa_ncnn/lib/libsherpa-ncnn-core.dylib
+-rwxr-xr-x  2.0 unx  8140320 b- defN 23-May-24 09:55 sherpa_ncnn/lib/libncnn.dylib
+-rwxr-xr-x  2.0 unx    96720 b- defN 23-May-24 09:55 sherpa_ncnn/lib/libkaldi-native-fbank-core.dylib
+-rw-rw-r--  2.0 unx     1067 b- defN 23-May-24 09:55 sherpa_ncnn-2.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx    11358 b- defN 23-May-24 09:55 sherpa_ncnn-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx      109 b- defN 23-May-24 09:55 sherpa_ncnn-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 23-May-24 09:55 sherpa_ncnn-2.0.2.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     2135 b- defN 23-May-24 09:55 sherpa_ncnn-2.0.2.dist-info/METADATA
+12 files, 8872395 bytes uncompressed, 3355250 bytes compressed:  62.2%
```

## zipnote {}

```diff
@@ -1,61 +1,37 @@
-Filename: _sherpa_ncnn.cp39-win_amd64.pyd
-Comment: 
-
-Filename: kaldi-native-fbank-core.dll
-Comment: 
-
-Filename: kaldi-native-fbank-core.lib
-Comment: 
-
-Filename: ncnn.dll
-Comment: 
-
-Filename: ncnn.lib
-Comment: 
-
-Filename: sherpa-ncnn-core.dll
-Comment: 
-
-Filename: sherpa-ncnn-core.lib
-Comment: 
-
-Filename: sherpa_ncnn/__init__.py
+Filename: _sherpa_ncnn.cpython-39-darwin.so
 Comment: 
 
 Filename: sherpa_ncnn/recognizer.py
 Comment: 
 
-Filename: sherpa_ncnn/bin/ncnn.dll
-Comment: 
-
-Filename: sherpa_ncnn/lib/kaldi-native-fbank-core.dll
+Filename: sherpa_ncnn/__init__.py
 Comment: 
 
-Filename: sherpa_ncnn/lib/kaldi-native-fbank-core.lib
+Filename: sherpa_ncnn/lib/libsherpa-ncnn-c-api.dylib
 Comment: 
 
-Filename: sherpa_ncnn/lib/ncnn.lib
+Filename: sherpa_ncnn/lib/libsherpa-ncnn-core.dylib
 Comment: 
 
-Filename: sherpa_ncnn/lib/sherpa-ncnn-c-api.dll
+Filename: sherpa_ncnn/lib/libncnn.dylib
 Comment: 
 
-Filename: sherpa_ncnn/lib/sherpa-ncnn-c-api.lib
+Filename: sherpa_ncnn/lib/libkaldi-native-fbank-core.dylib
 Comment: 
 
-Filename: sherpa_ncnn-2.0.1.dist-info/LICENSE
+Filename: sherpa_ncnn-2.0.2.dist-info/RECORD
 Comment: 
 
-Filename: sherpa_ncnn-2.0.1.dist-info/METADATA
+Filename: sherpa_ncnn-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: sherpa_ncnn-2.0.1.dist-info/WHEEL
+Filename: sherpa_ncnn-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sherpa_ncnn-2.0.1.dist-info/top_level.txt
+Filename: sherpa_ncnn-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sherpa_ncnn-2.0.1.dist-info/RECORD
+Filename: sherpa_ncnn-2.0.2.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## sherpa_ncnn/__init__.py

```diff
@@ -1,3 +1,3 @@
-from .recognizer import Recognizer
-from _sherpa_ncnn import Display
-__version__ = '2.0.1'
+from .recognizer import Recognizer
+from _sherpa_ncnn import Display
+__version__ = '2.0.2'
```

## sherpa_ncnn/recognizer.py

 * *Ordering differences only*

```diff
@@ -1,233 +1,233 @@
-from pathlib import Path
-
-import numpy as np
-from _sherpa_ncnn import (
-    DecoderConfig,
-    EndpointConfig,
-    FeatureExtractorConfig,
-    ModelConfig,
-)
-from _sherpa_ncnn import Recognizer as _Recognizer
-from _sherpa_ncnn import RecognizerConfig
-
-
-def _assert_file_exists(f: str):
-    assert Path(f).is_file(), f"{f} does not exist"
-
-
-class Recognizer(object):
-    """A class for streaming speech recognition.
-
-    Please refer to
-    `<https://k2-fsa.github.io/sherpa/ncnn/pretrained_models/index.html>`_
-    to download pre-trained models for different languages, e.g., Chinese,
-    English, etc.
-
-    **Usage example**
-
-    .. code-block:: python3
-
-        import wave
-
-        import numpy as np
-        import sherpa_ncnn
-
-
-        def main():
-            recognizer = sherpa_ncnn.Recognizer(
-                tokens="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/tokens.txt",
-                encoder_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/encoder_jit_trace-pnnx.ncnn.param",
-                encoder_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/encoder_jit_trace-pnnx.ncnn.bin",
-                decoder_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/decoder_jit_trace-pnnx.ncnn.param",
-                decoder_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/decoder_jit_trace-pnnx.ncnn.bin",
-                joiner_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/joiner_jit_trace-pnnx.ncnn.param",
-                joiner_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/joiner_jit_trace-pnnx.ncnn.bin",
-                num_threads=4,
-            )
-
-            filename = "./sherpa-ncnn-conv-emformer-transducer-2022-12-06/test_wavs/1.wav"
-            with wave.open(filename) as f:
-                assert f.getframerate() == recognizer.sample_rate, (
-                    f.getframerate(),
-                    recognizer.sample_rate,
-                )
-                assert f.getnchannels() == 1, f.getnchannels()
-                assert f.getsampwidth() == 2, f.getsampwidth()  # it is in bytes
-                num_samples = f.getnframes()
-                samples = f.readframes(num_samples)
-                samples_int16 = np.frombuffer(samples, dtype=np.int16)
-                samples_float32 = samples_int16.astype(np.float32)
-
-                samples_float32 = samples_float32 / 32768
-
-            recognizer.accept_waveform(recognizer.sample_rate, samples_float32)
-
-            tail_paddings = np.zeros(int(recognizer.sample_rate * 0.5), dtype=np.float32)
-            recognizer.accept_waveform(recognizer.sample_rate, tail_paddings)
-
-            recognizer.input_finished()
-
-            print(recognizer.text)
-
-
-        if __name__ == "__main__":
-            main()
-    """
-
-    def __init__(
-        self,
-        tokens: str,
-        encoder_param: str,
-        encoder_bin: str,
-        decoder_param: str,
-        decoder_bin: str,
-        joiner_param: str,
-        joiner_bin: str,
-        num_threads: int = 4,
-        decoding_method: str = "greedy_search",
-        num_active_paths: int = 4,
-        enable_endpoint_detection: bool = False,
-        rule1_min_trailing_silence: int = 2.4,
-        rule2_min_trailing_silence: int = 1.2,
-        rule3_min_utterance_length: int = 20,
-        model_sample_rate: int = 16000,
-    ):
-        """
-        Please refer to
-        `<https://k2-fsa.github.io/sherpa/ncnn/pretrained_models/index.html>`_
-        to download pre-trained models for different languages, e.g., Chinese,
-        English, etc.
-
-        Args:
-          tokens:
-            Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
-            columns::
-
-                symbol integer_id
-
-          encoder_param:
-            Path to ``encoder.ncnn.param``.
-          encoder_bin:
-            Path to ``encoder.ncnn.bin``.
-          decoder_param:
-            Path to ``decoder.ncnn.param``.
-          decoder_bin:
-            Path to ``decoder.ncnn.bin``.
-          joiner_param:
-            Path to ``joiner.ncnn.param``.
-          joiner_bin:
-            Path to ``joiner.ncnn.bin``.
-          num_threads:
-            Number of threads for neural network computation.
-          decoding_method:
-            Valid decoding methods are: greedy_search, modified_beam_search.
-          num_active_paths:
-            Used only when decoding_method is modified_beam_search. Its value
-            is ignored when decoding_method is greedy_search. It specifies
-            the maximum number of paths to use in beam search.
-          enable_endpoint_detection:
-            True to enable endpoint detection. False to disable endpoint
-            detection.
-          rule1_min_trailing_silence:
-            Used only when enable_endpoint_detection is True. If the duration
-            of trailing silence in seconds is larger than this value, we assume
-            an endpoint is detected.
-          rule2_min_trailing_silence:
-            Used only when enable_endpoint_detection is True. If we have decoded
-            something that is nonsilence and if the duration of trailing silence
-            in seconds is larger than this value, we assume an endpoint is
-            detected.
-          rule3_min_utterance_length:
-            Used only when enable_endpoint_detection is True. If the utterance
-            length in seconds is larger than this value, we assume an endpoint
-            is detected.
-          model_sample_rate:
-            Sample rate expected by the model
-        """
-        _assert_file_exists(tokens)
-        _assert_file_exists(encoder_param)
-        _assert_file_exists(encoder_bin)
-        _assert_file_exists(decoder_param)
-        _assert_file_exists(decoder_bin)
-        _assert_file_exists(joiner_param)
-        _assert_file_exists(joiner_bin)
-
-        assert num_threads > 0, num_threads
-        assert decoding_method in (
-            "greedy_search",
-            "modified_beam_search",
-        ), decoding_method
-        feat_config = FeatureExtractorConfig(
-            sampling_rate=model_sample_rate,
-            feature_dim=80,
-        )
-
-        model_config = ModelConfig(
-            encoder_param=encoder_param,
-            encoder_bin=encoder_bin,
-            decoder_param=decoder_param,
-            decoder_bin=decoder_bin,
-            joiner_param=joiner_param,
-            joiner_bin=joiner_bin,
-            num_threads=num_threads,
-            tokens=tokens,
-        )
-
-        endpoint_config = EndpointConfig(
-            rule1_min_trailing_silence=rule1_min_trailing_silence,
-            rule2_min_trailing_silence=rule2_min_trailing_silence,
-            rule3_min_utterance_length=rule3_min_utterance_length,
-        )
-
-        decoder_config = DecoderConfig(
-            method=decoding_method,
-            num_active_paths=num_active_paths,
-        )
-
-        self.config = RecognizerConfig(
-            feat_config=feat_config,
-            model_config=model_config,
-            decoder_config=decoder_config,
-            endpoint_config=endpoint_config,
-            enable_endpoint=enable_endpoint_detection,
-        )
-
-        self.sample_rate = self.config.feat_config.sampling_rate
-
-        self.recognizer = _Recognizer(self.config)
-        self.stream = self.recognizer.create_stream()
-
-    def accept_waveform(self, sample_rate: float, waveform: np.array):
-        """Decode audio samples.
-
-        Args:
-          sample_rate:
-            Sample rate of the input audio samples. You must use the same
-            value across different calls to `accept_waveform`! If it
-            is different from self.sample_rate, we will do resampling inside.
-          waveform:
-            A 1-D float32 array containing audio samples in the
-            range ``[-1, 1]``.
-        """
-        self.stream.accept_waveform(sample_rate, waveform)
-        self._decode()
-
-    def input_finished(self):
-        """Signal that no more audio samples are available."""
-        self.stream.input_finished()
-        self._decode()
-
-    def _decode(self):
-        while self.recognizer.is_ready(self.stream):
-            self.recognizer.decode_stream(self.stream)
-
-    @property
-    def text(self):
-        return self.recognizer.get_result(self.stream).text
-
-    @property
-    def is_endpoint(self):
-        return self.recognizer.is_endpoint(self.stream)
-
-    def reset(self):
-        self.recognizer.reset(self.stream)
+from pathlib import Path
+
+import numpy as np
+from _sherpa_ncnn import (
+    DecoderConfig,
+    EndpointConfig,
+    FeatureExtractorConfig,
+    ModelConfig,
+)
+from _sherpa_ncnn import Recognizer as _Recognizer
+from _sherpa_ncnn import RecognizerConfig
+
+
+def _assert_file_exists(f: str):
+    assert Path(f).is_file(), f"{f} does not exist"
+
+
+class Recognizer(object):
+    """A class for streaming speech recognition.
+
+    Please refer to
+    `<https://k2-fsa.github.io/sherpa/ncnn/pretrained_models/index.html>`_
+    to download pre-trained models for different languages, e.g., Chinese,
+    English, etc.
+
+    **Usage example**
+
+    .. code-block:: python3
+
+        import wave
+
+        import numpy as np
+        import sherpa_ncnn
+
+
+        def main():
+            recognizer = sherpa_ncnn.Recognizer(
+                tokens="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/tokens.txt",
+                encoder_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/encoder_jit_trace-pnnx.ncnn.param",
+                encoder_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/encoder_jit_trace-pnnx.ncnn.bin",
+                decoder_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/decoder_jit_trace-pnnx.ncnn.param",
+                decoder_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/decoder_jit_trace-pnnx.ncnn.bin",
+                joiner_param="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/joiner_jit_trace-pnnx.ncnn.param",
+                joiner_bin="./sherpa-ncnn-conv-emformer-transducer-2022-12-06/joiner_jit_trace-pnnx.ncnn.bin",
+                num_threads=4,
+            )
+
+            filename = "./sherpa-ncnn-conv-emformer-transducer-2022-12-06/test_wavs/1.wav"
+            with wave.open(filename) as f:
+                assert f.getframerate() == recognizer.sample_rate, (
+                    f.getframerate(),
+                    recognizer.sample_rate,
+                )
+                assert f.getnchannels() == 1, f.getnchannels()
+                assert f.getsampwidth() == 2, f.getsampwidth()  # it is in bytes
+                num_samples = f.getnframes()
+                samples = f.readframes(num_samples)
+                samples_int16 = np.frombuffer(samples, dtype=np.int16)
+                samples_float32 = samples_int16.astype(np.float32)
+
+                samples_float32 = samples_float32 / 32768
+
+            recognizer.accept_waveform(recognizer.sample_rate, samples_float32)
+
+            tail_paddings = np.zeros(int(recognizer.sample_rate * 0.5), dtype=np.float32)
+            recognizer.accept_waveform(recognizer.sample_rate, tail_paddings)
+
+            recognizer.input_finished()
+
+            print(recognizer.text)
+
+
+        if __name__ == "__main__":
+            main()
+    """
+
+    def __init__(
+        self,
+        tokens: str,
+        encoder_param: str,
+        encoder_bin: str,
+        decoder_param: str,
+        decoder_bin: str,
+        joiner_param: str,
+        joiner_bin: str,
+        num_threads: int = 4,
+        decoding_method: str = "greedy_search",
+        num_active_paths: int = 4,
+        enable_endpoint_detection: bool = False,
+        rule1_min_trailing_silence: int = 2.4,
+        rule2_min_trailing_silence: int = 1.2,
+        rule3_min_utterance_length: int = 20,
+        model_sample_rate: int = 16000,
+    ):
+        """
+        Please refer to
+        `<https://k2-fsa.github.io/sherpa/ncnn/pretrained_models/index.html>`_
+        to download pre-trained models for different languages, e.g., Chinese,
+        English, etc.
+
+        Args:
+          tokens:
+            Path to ``tokens.txt``. Each line in ``tokens.txt`` contains two
+            columns::
+
+                symbol integer_id
+
+          encoder_param:
+            Path to ``encoder.ncnn.param``.
+          encoder_bin:
+            Path to ``encoder.ncnn.bin``.
+          decoder_param:
+            Path to ``decoder.ncnn.param``.
+          decoder_bin:
+            Path to ``decoder.ncnn.bin``.
+          joiner_param:
+            Path to ``joiner.ncnn.param``.
+          joiner_bin:
+            Path to ``joiner.ncnn.bin``.
+          num_threads:
+            Number of threads for neural network computation.
+          decoding_method:
+            Valid decoding methods are: greedy_search, modified_beam_search.
+          num_active_paths:
+            Used only when decoding_method is modified_beam_search. Its value
+            is ignored when decoding_method is greedy_search. It specifies
+            the maximum number of paths to use in beam search.
+          enable_endpoint_detection:
+            True to enable endpoint detection. False to disable endpoint
+            detection.
+          rule1_min_trailing_silence:
+            Used only when enable_endpoint_detection is True. If the duration
+            of trailing silence in seconds is larger than this value, we assume
+            an endpoint is detected.
+          rule2_min_trailing_silence:
+            Used only when enable_endpoint_detection is True. If we have decoded
+            something that is nonsilence and if the duration of trailing silence
+            in seconds is larger than this value, we assume an endpoint is
+            detected.
+          rule3_min_utterance_length:
+            Used only when enable_endpoint_detection is True. If the utterance
+            length in seconds is larger than this value, we assume an endpoint
+            is detected.
+          model_sample_rate:
+            Sample rate expected by the model
+        """
+        _assert_file_exists(tokens)
+        _assert_file_exists(encoder_param)
+        _assert_file_exists(encoder_bin)
+        _assert_file_exists(decoder_param)
+        _assert_file_exists(decoder_bin)
+        _assert_file_exists(joiner_param)
+        _assert_file_exists(joiner_bin)
+
+        assert num_threads > 0, num_threads
+        assert decoding_method in (
+            "greedy_search",
+            "modified_beam_search",
+        ), decoding_method
+        feat_config = FeatureExtractorConfig(
+            sampling_rate=model_sample_rate,
+            feature_dim=80,
+        )
+
+        model_config = ModelConfig(
+            encoder_param=encoder_param,
+            encoder_bin=encoder_bin,
+            decoder_param=decoder_param,
+            decoder_bin=decoder_bin,
+            joiner_param=joiner_param,
+            joiner_bin=joiner_bin,
+            num_threads=num_threads,
+            tokens=tokens,
+        )
+
+        endpoint_config = EndpointConfig(
+            rule1_min_trailing_silence=rule1_min_trailing_silence,
+            rule2_min_trailing_silence=rule2_min_trailing_silence,
+            rule3_min_utterance_length=rule3_min_utterance_length,
+        )
+
+        decoder_config = DecoderConfig(
+            method=decoding_method,
+            num_active_paths=num_active_paths,
+        )
+
+        self.config = RecognizerConfig(
+            feat_config=feat_config,
+            model_config=model_config,
+            decoder_config=decoder_config,
+            endpoint_config=endpoint_config,
+            enable_endpoint=enable_endpoint_detection,
+        )
+
+        self.sample_rate = self.config.feat_config.sampling_rate
+
+        self.recognizer = _Recognizer(self.config)
+        self.stream = self.recognizer.create_stream()
+
+    def accept_waveform(self, sample_rate: float, waveform: np.array):
+        """Decode audio samples.
+
+        Args:
+          sample_rate:
+            Sample rate of the input audio samples. You must use the same
+            value across different calls to `accept_waveform`! If it
+            is different from self.sample_rate, we will do resampling inside.
+          waveform:
+            A 1-D float32 array containing audio samples in the
+            range ``[-1, 1]``.
+        """
+        self.stream.accept_waveform(sample_rate, waveform)
+        self._decode()
+
+    def input_finished(self):
+        """Signal that no more audio samples are available."""
+        self.stream.input_finished()
+        self._decode()
+
+    def _decode(self):
+        while self.recognizer.is_ready(self.stream):
+            self.recognizer.decode_stream(self.stream)
+
+    @property
+    def text(self):
+        return self.recognizer.get_result(self.stream).text
+
+    @property
+    def is_endpoint(self):
+        return self.recognizer.is_endpoint(self.stream)
+
+    def reset(self):
+        self.recognizer.reset(self.stream)
```

## Comparing `sherpa_ncnn-2.0.1.dist-info/LICENSE` & `sherpa_ncnn-2.0.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```


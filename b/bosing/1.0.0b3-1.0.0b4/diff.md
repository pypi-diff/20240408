# Comparing `tmp/bosing-1.0.0b3.tar.gz` & `tmp/bosing-1.0.0b4.tar.gz`

## Comparing `bosing-1.0.0b3.tar` & `bosing-1.0.0b4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
--rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.editorconfig
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.gitattributes
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.readthedocs.yaml
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.0b3/Bosing.sln
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.0b3/Directory.Build.props
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b3/VERSION.txt
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.0b3/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.0b3/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b3/exclusion.dic
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.github/dependabot.yml
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/Program.cs
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/__init__.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/_native.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/_utils.py
--rw-r--r--   0        0        0    18568 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/bosing/models.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/Makefile
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/api.rst
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/conf.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/index.rst
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/instruction.rst
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/make.bat
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/quickstart.rst
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/requirements.txt
--rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/schedule.rst
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/docs/_templates/autosummary/module.rst
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/example/schedule.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/example/schedule_stress.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 bosing-1.0.0b3/python/tests/test_basic.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadChain.cs
--rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadCoefficients.cs
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BiquadFilter.cs
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Bosing.csproj
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/BosingOptions.cs
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ComplexReadOnlySpan.cs
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ComplexSpan.cs
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Envelope.cs
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeCacheKey.cs
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeInfo.cs
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/EnvelopeSample.cs
--rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/FirCoefficients.cs
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/HannPulseShape.cs
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/IPulseShape.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/InterpolatedPulseShape.cs
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/IqPair.cs
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/MathUtils.cs
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PhaseTrackingTransform.cs
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PooledComplexArray.cs
--rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PostProcessTransform.cs
--rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/PulseList.cs
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/SignalFilter.cs
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/TimeAxisUtils.cs
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/TrianglePulseShape.cs
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/ValueArray.cs
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/WaveformSampler.cs
--rw-r--r--   0        0        0    29862 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/WaveformUtils.cs
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/AbsoluteSchedule.cs
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Alignment.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ArrangeOption.cs
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/BarrierElement.cs
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridLength.cs
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridLengthUnit.cs
--rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/GridSchedule.cs
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/PlayElement.cs
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/RepeatElement.cs
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Schedule.cs
--rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ScheduleElement.cs
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SetFrequencyElement.cs
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SetPhaseElement.cs
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ShiftFrequencyElement.cs
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/ShiftPhaseElement.cs
--rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/StackSchedule.cs
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/SwapPhaseElement.cs
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing/Schedules/Thickness.cs
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Api.cs
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Bosing.Aot.csproj
--rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/ScheduleRunner.cs
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/UnsafeMemoryManager.cs
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/BarrierElementDto.cs
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/BiquadDto.cs
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ChannelInfo.cs
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/GridScheduleDto.cs
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/HannShapeInfo.cs
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/IqCalibration.cs
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/OptionsDto.cs
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/PlayElementDto.cs
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/RepeatElementDto.cs
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleElementDto.cs
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleRequest.cs
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SetPhaseElementDto.cs
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShapeInfo.cs
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/StackScheduleDto.cs
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.0b3/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Bosing.Tests.csproj
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/EnvelopeInfoTests.cs
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/HannPulseShapeTests.cs
--rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/IntegrationTests.cs
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/IqPairTests.cs
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/MathUtilsTests.cs
--rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/PooledComplexArrayTests.cs
--rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/PulseListTests.cs
--rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/TimeAxisUtilsTests.cs
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/ToleranceComparer.cs
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/TrianglePulseShapeTests.cs
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Usings.cs
--rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/WaveformUtilsTests.cs
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
--rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleTests.cs
--rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.0b3/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.0b3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.0b3/LICENSE.txt
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bosing-1.0.0b3/README.md
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 bosing-1.0.0b3/hatch_build.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bosing-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 bosing-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0    17327 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.editorconfig
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.gitattributes
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.readthedocs.yaml
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 bosing-1.0.0b4/Bosing.sln
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 bosing-1.0.0b4/Directory.Build.props
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b4/VERSION.txt
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 bosing-1.0.0b4/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 bosing-1.0.0b4/WaveGenBenchmarks.WaveformUtilsBench-report-github.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bosing-1.0.0b4/exclusion.dic
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.github/dependabot.yml
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/Program.cs
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveGenBenchmarks.csproj
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveformUtilsBench.cs
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/__init__.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/_native.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/_utils.py
+-rw-r--r--   0        0        0    18568 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/bosing/models.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/Makefile
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/api.rst
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/conf.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/index.rst
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/instruction.rst
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/make.bat
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/quickstart.rst
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/requirements.txt
+-rw-r--r--   0        0        0     5572 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/schedule.rst
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/docs/_templates/autosummary/module.rst
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/example/schedule.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/example/schedule_stress.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bosing-1.0.0b4/python/tests/test_basic.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadChain.cs
+-rw-r--r--   0        0        0      775 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadCoefficients.cs
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BiquadFilter.cs
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Bosing.csproj
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/BosingOptions.cs
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ComplexReadOnlySpan.cs
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ComplexSpan.cs
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Envelope.cs
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeCacheKey.cs
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeInfo.cs
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/EnvelopeSample.cs
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/FirCoefficients.cs
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/HannPulseShape.cs
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/IPulseShape.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/InterpolatedPulseShape.cs
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/IqPair.cs
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/MathUtils.cs
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PhaseTrackingTransform.cs
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PooledComplexArray.cs
+-rw-r--r--   0        0        0     5917 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PostProcessTransform.cs
+-rw-r--r--   0        0        0     8270 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/PulseList.cs
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/SignalFilter.cs
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/TimeAxisUtils.cs
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/TrianglePulseShape.cs
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/ValueArray.cs
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/WaveformSampler.cs
+-rw-r--r--   0        0        0    30123 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/WaveformUtils.cs
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/AbsoluteSchedule.cs
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Alignment.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ArrangeOption.cs
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/BarrierElement.cs
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridLength.cs
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridLengthUnit.cs
+-rw-r--r--   0        0        0     6528 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/GridSchedule.cs
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/PlayElement.cs
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/RepeatElement.cs
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Schedule.cs
+-rw-r--r--   0        0        0     4884 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ScheduleElement.cs
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SetFrequencyElement.cs
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SetPhaseElement.cs
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ShiftFrequencyElement.cs
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/ShiftPhaseElement.cs
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/StackSchedule.cs
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/SwapPhaseElement.cs
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing/Schedules/Thickness.cs
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Api.cs
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Bosing.Aot.csproj
+-rw-r--r--   0        0        0     2878 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/ScheduleRunner.cs
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/UnsafeMemoryManager.cs
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/BarrierElementDto.cs
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/BiquadDto.cs
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ChannelInfo.cs
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/GridScheduleDto.cs
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/HannShapeInfo.cs
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/InterpolatedShapeInfo.cs
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/IqCalibration.cs
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/OptionsDto.cs
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/PlayElementDto.cs
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/RepeatElementDto.cs
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleElementDto.cs
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleRequest.cs
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SetFrequencyElementDto.cs
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SetPhaseElementDto.cs
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShapeInfo.cs
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/StackScheduleDto.cs
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 bosing-1.0.0b4/src/Bosing.Aot/Models/SwapPhaseElementDto.cs
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Bosing.Tests.csproj
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/EnvelopeInfoTests.cs
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/HannPulseShapeTests.cs
+-rw-r--r--   0        0        0     3251 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/IntegrationTests.cs
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/IqPairTests.cs
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/MathUtilsTests.cs
+-rw-r--r--   0        0        0     7704 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/PooledComplexArrayTests.cs
+-rw-r--r--   0        0        0     6888 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/PulseListTests.cs
+-rw-r--r--   0        0        0     4227 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/TimeAxisUtilsTests.cs
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/ToleranceComparer.cs
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/TrianglePulseShapeTests.cs
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Usings.cs
+-rw-r--r--   0        0        0    10320 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/WaveformUtilsTests.cs
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/GridScheduleTests.cs
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/RepeatElementTests.cs
+-rw-r--r--   0        0        0     6696 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleTests.cs
+-rw-r--r--   0        0        0     8670 2020-02-02 00:00:00.000000 bosing-1.0.0b4/tests/Bosing.Tests/Schedules/StackScheduleTests.cs
+-rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 bosing-1.0.0b4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 bosing-1.0.0b4/LICENSE.txt
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 bosing-1.0.0b4/README.md
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 bosing-1.0.0b4/hatch_build.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 bosing-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 bosing-1.0.0b4/PKG-INFO
```

### Comparing `bosing-1.0.0b3/.editorconfig` & `bosing-1.0.0b4/.editorconfig`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/.gitattributes` & `bosing-1.0.0b4/.gitattributes`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/.readthedocs.yaml` & `bosing-1.0.0b4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/Bosing.sln` & `bosing-1.0.0b4/Bosing.sln`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md` & `bosing-1.0.0b4/WaveGenBenchmarks.EnvelopeCacheBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/WaveGenBenchmarks.WaveformUtilsBench-report-github.md` & `bosing-1.0.0b4/WaveGenBenchmarks.WaveformUtilsBench-report-github.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/.github/workflows/ci.yml` & `bosing-1.0.0b4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs` & `bosing-1.0.0b4/examples/WaveGenBenchmarks/EnvelopeCacheBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/examples/WaveGenBenchmarks/WaveformUtilsBench.cs` & `bosing-1.0.0b4/examples/WaveGenBenchmarks/WaveformUtilsBench.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/bosing/__init__.py` & `bosing-1.0.0b4/python/bosing/__init__.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/bosing/_native.py` & `bosing-1.0.0b4/python/bosing/_native.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/bosing/_utils.py` & `bosing-1.0.0b4/python/bosing/_utils.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/bosing/models.py` & `bosing-1.0.0b4/python/bosing/models.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/Makefile` & `bosing-1.0.0b4/python/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/conf.py` & `bosing-1.0.0b4/python/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/instruction.rst` & `bosing-1.0.0b4/python/docs/instruction.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/make.bat` & `bosing-1.0.0b4/python/docs/make.bat`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/quickstart.rst` & `bosing-1.0.0b4/python/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/schedule.rst` & `bosing-1.0.0b4/python/docs/schedule.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/docs/_templates/autosummary/module.rst` & `bosing-1.0.0b4/python/docs/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/example/schedule.py` & `bosing-1.0.0b4/python/example/schedule.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/python/example/schedule_stress.py` & `bosing-1.0.0b4/python/example/schedule_stress.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/BiquadChain.cs` & `bosing-1.0.0b4/src/Bosing/BiquadChain.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/BiquadCoefficients.cs` & `bosing-1.0.0b4/src/Bosing/BiquadCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/BiquadFilter.cs` & `bosing-1.0.0b4/src/Bosing/BiquadFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Bosing.csproj` & `bosing-1.0.0b4/src/Bosing/Bosing.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/BosingOptions.cs` & `bosing-1.0.0b4/src/Bosing/BosingOptions.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/ComplexReadOnlySpan.cs` & `bosing-1.0.0b4/src/Bosing/ComplexReadOnlySpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/ComplexSpan.cs` & `bosing-1.0.0b4/src/Bosing/ComplexSpan.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Envelope.cs` & `bosing-1.0.0b4/src/Bosing/Envelope.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/EnvelopeInfo.cs` & `bosing-1.0.0b4/src/Bosing/EnvelopeInfo.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/EnvelopeSample.cs` & `bosing-1.0.0b4/src/Bosing/EnvelopeSample.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/FirCoefficients.cs` & `bosing-1.0.0b4/src/Bosing/FirCoefficients.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/HannPulseShape.cs` & `bosing-1.0.0b4/src/Bosing/HannPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/IPulseShape.cs` & `bosing-1.0.0b4/src/Bosing/IPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/InterpolatedPulseShape.cs` & `bosing-1.0.0b4/src/Bosing/InterpolatedPulseShape.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/IqPair.cs` & `bosing-1.0.0b4/src/Bosing/IqPair.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/MathUtils.cs` & `bosing-1.0.0b4/src/Bosing/MathUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/PhaseTrackingTransform.cs` & `bosing-1.0.0b4/src/Bosing/PhaseTrackingTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/PooledComplexArray.cs` & `bosing-1.0.0b4/src/Bosing/PooledComplexArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/PostProcessTransform.cs` & `bosing-1.0.0b4/src/Bosing/PostProcessTransform.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/PulseList.cs` & `bosing-1.0.0b4/src/Bosing/PulseList.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/SignalFilter.cs` & `bosing-1.0.0b4/src/Bosing/SignalFilter.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/TimeAxisUtils.cs` & `bosing-1.0.0b4/src/Bosing/TimeAxisUtils.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/ValueArray.cs` & `bosing-1.0.0b4/src/Bosing/ValueArray.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/WaveformSampler.cs` & `bosing-1.0.0b4/src/Bosing/WaveformSampler.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/WaveformUtils.cs` & `bosing-1.0.0b4/src/Bosing/WaveformUtils.cs`

 * *Files 2% similar despite different names*

```diff
@@ -113,21 +113,27 @@
 
     private static void MixAddEnvelope<T>(ComplexSpan<T> target, EnvelopeSample<T> envelopeSample, IqPair<T> complexAmplitude, IqPair<T> dragAmplitude, T dPhase) where T : unmanaged, IFloatingPointIeee754<T>
     {
         var currentIndex = 0;
 
         var leftEdge = envelopeSample.LeftEdge;
         MixAdd(target[currentIndex..], leftEdge, complexAmplitude, dragAmplitude, dPhase);
-        currentIndex += leftEdge.Length;
-
+        ShiftIndex(leftEdge.Length);
         MixAddPlateau(target.Slice(currentIndex, envelopeSample.Plateau), complexAmplitude, dPhase);
-        currentIndex += envelopeSample.Plateau;
-
+        ShiftIndex(envelopeSample.Plateau);
         var rightEdge = envelopeSample.RightEdge;
         MixAdd(target[currentIndex..], rightEdge, complexAmplitude, dragAmplitude, dPhase);
+
+        void ShiftIndex(int count)
+        {
+            currentIndex += count;
+            var phaseInc = IqPair<T>.FromPolarCoordinates(T.One, dPhase * T.CreateChecked(count));
+            complexAmplitude *= phaseInc;
+            dragAmplitude *= phaseInc;
+        }
     }
 
     public static void MixAddPlateau<T>(ComplexSpan<T> target, IqPair<T> amplitude, T dPhase)
         where T : unmanaged, IFloatingPointIeee754<T>
     {
         if (target.Length == 0)
         {
```

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/AbsoluteSchedule.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/AbsoluteSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/BarrierElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/BarrierElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/GridLength.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/GridLength.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/GridSchedule.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/GridSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/PlayElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/PlayElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/RepeatElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/RepeatElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/Schedule.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/Schedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/ScheduleElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/ScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/SetFrequencyElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/SetFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/SetPhaseElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/SetPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/ShiftFrequencyElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/ShiftFrequencyElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/ShiftPhaseElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/ShiftPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/StackSchedule.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/StackSchedule.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing/Schedules/SwapPhaseElement.cs` & `bosing-1.0.0b4/src/Bosing/Schedules/SwapPhaseElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Api.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Api.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Bosing.Aot.csproj` & `bosing-1.0.0b4/src/Bosing.Aot/Bosing.Aot.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/ScheduleRunner.cs` & `bosing-1.0.0b4/src/Bosing.Aot/ScheduleRunner.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/AbsoluteScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/BarrierElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/BarrierElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/BiquadDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/BiquadDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/GridScheduleDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/GridScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/OptionsDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/OptionsDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/PlayElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/PlayElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/RepeatElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/RepeatElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/ScheduleElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/ScheduleElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/SetFrequencyElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/SetFrequencyElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/SetPhaseElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/SetPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftFrequencyElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/ShiftPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/StackScheduleDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/StackScheduleDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/src/Bosing.Aot/Models/SwapPhaseElementDto.cs` & `bosing-1.0.0b4/src/Bosing.Aot/Models/SwapPhaseElementDto.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Bosing.Tests.csproj` & `bosing-1.0.0b4/tests/Bosing.Tests/Bosing.Tests.csproj`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/ComplexReadOnlySpanTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/EnvelopeInfoTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/EnvelopeInfoTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/HannPulseShapeTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/HannPulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/IntegrationTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/IntegrationTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/IqPairTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/IqPairTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/PooledComplexArrayTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/PooledComplexArrayTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/PulseListTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/PulseListTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/TimeAxisUtilsTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/TimeAxisUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/TrianglePulseShapeTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/TrianglePulseShapeTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/WaveformUtilsTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/WaveformUtilsTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/AbsoluteScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/FakeScheduleElement.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/GridScheduleTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/GridScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/RepeatElementTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/RepeatElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleElementTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/ScheduleTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/ScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/tests/Bosing.Tests/Schedules/StackScheduleTests.cs` & `bosing-1.0.0b4/tests/Bosing.Tests/Schedules/StackScheduleTests.cs`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/.gitignore` & `bosing-1.0.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/LICENSE.txt` & `bosing-1.0.0b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/README.md` & `bosing-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/hatch_build.py` & `bosing-1.0.0b4/hatch_build.py`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/pyproject.toml` & `bosing-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bosing-1.0.0b3/PKG-INFO` & `bosing-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bosing
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: Waveform generator for pulse sequences in quantum computing
 Project-URL: Documentation, https://github.com/kahojyun/Bosing#readme
 Project-URL: Issues, https://github.com/kahojyun/Bosing/issues
 Project-URL: Source, https://github.com/kahojyun/Bosing
 Author-email: kaho <kaho0769@qq.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


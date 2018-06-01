load("@io_tweag_rules_haskell//haskell:haskell.bzl", "haskell_library")

haskell_library(
  name = "memory",
  visibility = ["//visibility:public"],
  deps = [
    "@hackage_basement//:basement",
    "@hackage_foundation//:foundation",
  ],
  prebuilt_dependencies = [
    "bytestring",
    "base",
    "ghc-prim",
    "deepseq",
  ],
  compiler_flags = [
    "-DWITH_BYTESTRING_SUPPORT",
    "-DWITH_DEEPSEQ_SUPPORT",
    "-DWITH_FOUNDATION_SUPPORT",
  ],
  srcs = [
    "Data/ByteArray.hs",
    "Data/ByteArray/Encoding.hs",
    "Data/ByteArray/Mapping.hs",
    "Data/ByteArray/Pack.hs",
    "Data/ByteArray/Parse.hs",
    "Data/ByteArray/Hash.hs",
    "Data/Memory/Endian.hs",
    "Data/Memory/PtrMethods.hs",
    "Data/Memory/ExtendedWords.hs",
    "Data/Memory/Encoding/Base16.hs",
    "Data/Memory/Encoding/Base32.hs",
    "Data/Memory/Encoding/Base64.hs",
    "Data/Memory/Internal/Compat.hs",
    "Data/Memory/Internal/CompatPrim.hs",
    "Data/Memory/Internal/CompatPrim64.hs",
    "Data/Memory/Internal/DeepSeq.hs",
    "Data/Memory/Internal/Imports.hs",
    "Data/Memory/Internal/Scrubber.hs",
    "Data/Memory/Hash/SipHash.hs",
    "Data/Memory/Hash/FNV.hs",
    "Data/ByteArray/Pack/Internal.hs",
    "Data/ByteArray/Types.hs",
    "Data/ByteArray/Bytes.hs",
    "Data/ByteArray/ScrubbedBytes.hs",
    "Data/ByteArray/Methods.hs",
    "Data/ByteArray/MemView.hs",
    "Data/ByteArray/View.hs",
    "Data/Memory/MemMap/Posix.hsc",
  ],
)
